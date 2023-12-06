# Medidor de Temperatura com Comunicação Serial I2C

O projeto do Medidor de Temperatura com Display LED I2C é uma solução eficiente para monitoramento de temperatura em tempo real. Este projeto foi desenvolvido utilizando o microcontrolador Raspberry Pi Pico, conhecido pela sua versatilidade, juntamente com um sensor de temperatura e um display LED I2C para uma visualização clara e direta.

O objetivo deste projeto é fornecer um dispositivo confiável e fácil de usar para medir temperaturas em diferentes ambientes, como em casa, escritórios, carros ou até mesmo saídas de ar de nossos computadores, como foi visto nos vídeos anteriores. Através de uma interface simplificada, o usuário pode obter leituras de temperatura precisas e instantâneas, exibidas de maneira clara no display LED I2C.

Este documento README destina-se a fornecer todas as informações necessárias para compreender, montar e operar o Medidor de Temperatura com Display LED I2C. Aqui você encontrará detalhes sobre o hardware utilizado, a descrição do funcionamento da comunicação I2C e serial, além de um vídeo demonstrativo que ilustra o funcionamento prático do projeto.

## Conteúdo
- [Descrição do Hardware](#descrição-do-hardware)
- [Comunicação I2C e Serial](#comunicação-i2c-e-serial)
- [Vídeo Demonstrativo](#vídeo-demonstrativo)
- [Como Usar](#como-usar)
- [Licença](#licença)

## Descrição do Hardware

### Diagrama de Blocos

![Diagrama de Blocos](caminho/para/o/diagrama.png)

Detalhes do diagrama de blocos mostrando a pinagem entre o microcontrolador Raspberry Pi Pico e o sensor I2C.

## Comunicação I2C e Serial

### Comunicação I2C

Explicação de como o Raspberry Pi Pico se comunica com o sensor I2C, incluindo detalhes técnicos sobre o protocolo I2C.

### Comunicação Serial

A comunicação serial entre o computador e o microcontrolador, como o Raspberry Pi Pico, é uma maneira fundamental de trocar dados entre esses dispositivos. Este processo envolve usar uma das interfaces de comunicação serial do Raspberry Pi Pico, tipicamente UART (Universal Asynchronous Receiver/Transmitter), para transmitir e receber dados.

Primeiro, é necessário configurar a interface serial no Raspberry Pi Pico. Isso envolve definir os pinos para transmissão (TX) e recepção (RX) de dados, além de configurar a taxa de transmissão (baud rate), que deve ser a mesma no microcontrolador e no computador. A conexão física pode ser feita diretamente através de um cabo USB, se o Raspberry Pi Pico suportar comunicação serial sobre USB, ou através de um adaptador USB para TTL (Transistor-Transistor Logic) se uma conexão direta não for possível.

Uma vez estabelecida a conexão, o microcontrolador pode enviar dados para o computador. Isso é feito escrevendo dados no buffer de transmissão da UART. Quando o buffer é preenchido, os dados são enviados sequencialmente através do pino TX. De maneira similar, o microcontrolador pode receber dados do computador. Os dados enviados pelo computador são recebidos no pino RX do microcontrolador e armazenados no buffer de recepção da UART. O microcontrolador pode então ler esses dados.

(REZENDE, R. Raspberry Pi - Comunicação Serial (UART) entre a Raspberry Pi e Arduino em Python e Wiring. Disponível em: <https://embarcados.com.br/raspberry-pi-comunicacao-serial-uart/>.)

## Vídeo Demonstrativo

Link para o vídeo-pitch (será adicionado posteriormente).

Descrição do que é mostrado no vídeo, incluindo demonstração do funcionamento do microcontrolador e sensor e a impressão de dados no terminal da IDE.

## Como Usar

Instruções passo a passo sobre como configurar e usar o sistema.

## Licença

Informações sobre a licença do projeto.
