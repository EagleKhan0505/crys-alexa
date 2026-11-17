# Crys e Alexa

**Uma integração para conversar com IA pela Alexa.**

[English](README.en.md) · [Gustavo Amaral](https://github.com/EagleKhan0505)

## A ideia

Quis levar a experiência de conversar com uma assistente de IA para uma interface por voz. A Crys conecta uma skill da Alexa à API da OpenAI, permitindo formular perguntas em português e receber respostas curtas, adequadas à conversa falada.

## O que foi construído

- Skill personalizada em português do Brasil, com abertura, perguntas, ajuda e encerramento.
- Integração da Alexa com a API da OpenAI em um backend Node.js hospedado na nuvem.
- Contexto curto de sessão para dar continuidade à conversa.
- Busca web com fontes apresentadas no cartão da resposta.
- Tratamento de falhas e limites de tempo compatíveis com uma interação por voz.
- Recuperação da credencial em serviço de segredos, sem chave embutida no código.

```mermaid
flowchart LR
    A[Pergunta pela Alexa] --> B[Skill Crys]
    B --> C[API da OpenAI]
    C --> D[Resposta curta em português]
    D --> A
```

## Minha contribuição

Defini a experiência desejada, conduzi a integração com apoio de IA e acompanhei os testes e a investigação de falhas. O desenvolvimento envolve transformar uma conversa em um fluxo que precisa lidar com reconhecimento de pedidos, contexto, tempo de resposta e serviços externos.

## Estado atual

Protótipo implantado no ambiente de desenvolvimento da Alexa. Perguntas e busca com fontes foram exercitadas no simulador; o funcionamento por voz no Echo físico ainda precisa de validação completa. O projeto utiliza a API da OpenAI e não acessa as conversas ou memórias da conta do ChatGPT.

**Tecnologias:** Node.js, Alexa Skills, OpenAI API, AWS STS e Secrets Manager.

Este repositório apresenta a integração. Código, credenciais, identificadores de infraestrutura e configurações da conta permanecem privados.
