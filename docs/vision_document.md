# Documento de Visão

## Histórico de Versão
| Data | Versão | Descrição | Autor |
| :--- | :--- | :--- | :--- |
| 18/08| 0.1 | Adicionado Introdução| João Vitor, João Pedro, Lucas Midley e Lucas Oliveira |

## Sumário
[1. Introdução] (#1-introdução)
* [1.1 Sobre o RPG de mesa](#11-sobre-o-rog-de-mesa)
* [1.2 Objetivo](#12-objetivo)
* [1.3 Visão Geral da Solução](#13-visão-geral-da-solução)

## 1. Introdução

Este documento tem o objetivo de definir os aspectos relevantes do projeto e levantar os requisitos necessários para executá-lo.
A ideia base deste projeto consiste na criação de um _chatbot_ que automatize um dos aspectos de um RPG de mesa utilizando a plataforma de serviço de mensagens _Telegram_.

### 1.1 Sobre o RPG de mesa

O RPG (do inglês, _Role Playing Game_) de mesa é um genêro jogo colaborativo em que os jogadores assumem papéis de personagens em um ambiente imaginário para criar uma história seguindo regras e diretrizes pré-definidas. As partidas, normalmente, ocorrem em sessões em que esses jogadores se reúnem para jogar. 

Além disso, é possível realizar ações durante essas sessões, como comprar ou usar itens, aprender uma nova habilidade etc. Nesses casos, os jogadores precisam conversar com o Mestre para saber se é possível realizar as ações desejadas. Porém, por depender exclusivamente do Mestre para a execução do jogo, este pode ficar sobrecarregado a depender da quantidade de ações e/ou jogadores.

### 1.2 Objetivo

Este projeto tem como objetivo central facilitar o gerenciamento de trocas de itens feitas pelos jogadores no intervalo entre as sessões.

Atualmente, toda a gerência de estoque de lojas dos NPC's(Personagens Não Jogáveis) e coleta de impostos na cidade onde o jogo se passa, é feita pelo Mestre. O que ocorre em demora no tempo de resposta e possíveis erros.

### 1.3 Visão Geral da Solução

O propósito do _chatbot_ é automatizar o processo de compra e venda de itens entre os jogadores e os NPC's, além de gerar um relatório das vendas para o Mestre. O sistema também será responsável pela troca de itens entre os NPC's e por fazer a coleta de impostos destes.

| O problema da| Centralização de tarefas|
| :--- | :---: |
| Afeta | Os jogadores e, principalmente, o Mestre. |
| Cujo impacto é | O atraso da resposta e possíveis erros por parte do Mestre |
| Uma boa solução seria | Um _chatbot_ que descentralize as responsilidades do Mestre.|