# Projetos-com-python
criando IA com python e Projetos com python
from openai import OpenAI

cliente = OpenAI(
    api_key="",
    base_url="https://integrate.api.nvidia.com/v1"
)

historico_conversa = [
    {
        "role": "system",
        "content": "Voce e um divertido amigo, responda de forma carinhosa"
    }
]

print("Sou seu amigo chatbot, digite 'sair' para encerrar nossa conversa")

while True:
    pergunta_usuario = input("Voce: ")
    if pergunta_usuario.lower() == "sair":
        print("Ate mais!")
        break

    historico_conversa.append({
        "role": "user",
        "content": pergunta_usuario
    })

    resposta_ai = cliente.chat.completions.create(
        model="meta/llama-3.1-8b-instruct",
        messages=historico_conversa
    )

    conteudo_resposta = resposta_ai.choices[0].message.content

    print(f"Amigo chatbot: {conteudo_resposta}")

    historico_conversa.append({
        "role": "assistant",
        "content": conteudo_resposta
    })
        
