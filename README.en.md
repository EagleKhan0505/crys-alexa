# Crys and Alexa

**An experimental integration for talking to AI through Alexa.**

[Português](README.md) · [Gustavo Amaral](https://github.com/EagleKhan0505)

## Motivation

I wanted to bring an AI-assistant experience to a voice interface. Crys connects a custom Alexa skill to the OpenAI API, accepting questions in Brazilian Portuguese and returning short responses suited to speech.

## Implemented capabilities

- Custom skill with launch, question, help and exit interactions.
- Cloud-hosted Node.js integration with the OpenAI API.
- Short session context for follow-up conversation.
- Web search with sources included in the response card.
- Error handling and time limits for the voice interaction.
- Secret retrieval without embedding a credential in the source code.

## My contribution

I defined the intended experience, guided AI-assisted integration and reviewed tests and failure reports. The work brings together intent handling, conversational context, response timing and external services.

## Current stage

A prototype deployed in Alexa's development environment. Questions and source-backed search were exercised in the simulator; end-to-end voice behavior on a physical Echo still requires full validation. The integration uses the OpenAI API and does not access ChatGPT account conversations or memories.

**Technologies:** Node.js, Alexa Skills, OpenAI API, AWS STS and Secrets Manager.

This repository presents the integration. Implementation, credentials, infrastructure identifiers and account configuration remain private.
