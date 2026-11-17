# Projetos em Python — Chatbot com IA

**Autor:** Kaiky Yoshio Ono Marins  
**Categoria:** Python · Inteligência Artificial  
**Status:** Experimento de estudo

## Visão geral

Exemplo de chatbot executado no terminal. O programa envia mensagens para um modelo de linguagem por meio de um endpoint compatível com a API da OpenAI e mantém o histórico da conversa em memória enquanto o processo está aberto.

## O que o exemplo demonstra

- Entrada e saída de mensagens pelo terminal.
- Construção de uma conversa com papéis `system`, `user` e `assistant`.
- Envio do histórico para o modelo a cada interação.
- Encerramento da conversa por comando.

## Tecnologias

- Python
- SDK `openai`
- Endpoint compatível da NVIDIA NIM
- Modelo de linguagem Llama

## Material e execução

O exemplo original está preservado em [MATERIAL-ORIGINAL.txt](./MATERIAL-ORIGINAL.txt). Antes de executar, instale a dependência `openai` e configure sua chave de API de forma segura no ambiente local. O trecho arquivado usa uma chave vazia como marcador e precisa dessa configuração para funcionar.

**Segurança:** nunca grave chaves de API no código, no README ou em commits.

© 2026 Kaiky Yoshio Ono Marins.