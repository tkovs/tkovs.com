---
title: Correios Tracking
summary: Um gerenciador de rastreios de encomendas dos Correios
tags:
- Data Tracking
date: "2019-10-07T03:40:00Z"
---

Gerenciador de rastreios de encomendas transportadas pelos Correios.

### Recursos

Rastreie e acompanhe movimentações de suas encomendas. Arquive ou delete aquelas que não lhe interessam mais. Nomeie cada rastreio encomenda para diferenciar todas as suas encomendas. Filtre por encomendas pendentes e encomenda entregues.

### Tecnologias

O projeto foi escrito em Javascript utilizando
- **React Native** para que o app possa rodar em plataforma mobile sem necessidade de escrever código nativo.
- **ReactJS** para componentização, padrão no React Native.
- **TypeScript** para lidar com tipos de variáveis e funções, aumentando a confiabilidade do código e quantidade de erros pegos em tempo de desenvolvimento.
- **Redux** para gerenciamento de estado global
- **React Native Testing Library** para testes automatizandos unitários de componentes
- **Detox** para testes automatizados de fluxos end-to-end
- **Encomendas Correios** é um pacote npm que eu criei rapidamente para que esse app funcione. Esse pacote utiliza um código de rastreio para puxar informações sobre uma encomenda.

### Próximos passos

- [ ] Internacionalizar as mensagens
- [ ] Notificar o dispositivo quando houver atualizações das encomendas

### Seja um contribuidor

Seu código fonte é publico e está em [meu github](https://github.com/tkovs/correios-app), livre para forks e contribuições. Para executar, basta seguir os passos descritos no README do repositório.

## Demonstração

No gif abaixo eu mostro o projeto sendo executado.

![App demo](demo.gif)
