---
layout: faq
title: FAQ
description: Respostas para perguntas frequentes feitas pelos desenvolvedores durante a integração com a Cielo LIO.
search: true
categories: faq
tags:
  - Cielo LIO
search: true
---

# Dúvidas Plataforma LIO

## Se o estabelecimento comercial trocar a LIO v1 pela LIO v2, o que ele precisa fazer para ter o aplicativo na nova máquina?

Ao receber o novo equipamento, o cliente deve garantir que a LIO esteja conectada no 3G ou no Wi-Fi e então solicitar para atualizar aplicativos.

Ajuda -> Sobre Cielo LIO -> Atualizar Aplicativos Cielo LIO

Após esse procedimento todos os aplicativos que o cliente possui serão transferidos também para a nova máquina.

## É necessário fazer uma nova certificação do meu aplicativo para que ele funcione na LIO v2?

Não, se o aplicativo já foi certificado não tem a necessidade de certificar novamente, exceto no caso de o desenvolvedor utilizar em seu aplicativo métodos e/ou funcionalidades exclusivas da LIO V2. Então ele deverá submeter o aplicativo para certificação.

## Se o estabelecimento comercial possui máquinas LIO v1 como também LIO v2, o aplicativo do parceiro vai funcionar em ambas?

Sim, o aplicativo do parceiro irá funcionar em ambos os modelos de LIO (V1 e V2).

## Se meu aplicativo já funciona na LIO v1, ele vai funcionar também na LIO v2?

Sim, se você já tem um aplicativo rodando na LIO V1, ele também funcionará na LIO V2.

## Como faço para integrar com a Cielo LIO?

Construimos um portal dedicado aos desenvolvedores para facilitar a integração da sua solução com a Lio:

> http://desenvolvedores.cielo.com.br

Nesse portal você pode:

* Acessar documentação completa das APIs
* Utilizar os SDK´s para tornar a integração mais ágil
* Criar suas contas para receber as chaves (tokens) de acesso
* Realizar os testes e desenvolvimentos para se integrarem com a Cielo: usando emulador ou sandbox.

## Posso utilizar impressoras para conectar na Cielo LIO?

Sim. Impressoras com conexão via Bluetooth podem ser usadas pelo aplicativo do parceiro que está rodando na Cielo LIO para realizar a impressão de algum comprovante ou recibo necessário para a operação do negócio do parceiro/cliente.
Já existem parceiros que estão utilizando impressoras Bluetooth das marcas Zebra, Datex, Leopardo e outras para se integrar com a Cielo LIO!
Todos os protocolos de comunicação e pareamento ficam sob responsabilidade do aplicativo do parceiro.

## Quais são as formas de comunicação da Cielo LIO?

A Cielo LIO possui entrada para um SIM Card que permite realizar a comunicação via rede móvel 3G. Com fall-back para 2G e GPRS respectivamente.
Além disso, ela possui como tecnologia de comunicação o Wi-Fi.

## Quais são as conexões disponíveis na Cielo LIO?

As entradas USB da Cielo LIO são utilizadas única e exclusivamente para realizar o carregamento na bateria do aparelho.
O Bluetooth da Cielo LIO pode ser utilizado para realizar a comunicação e a troca de informações com dispositivos externos.

## A minha máquina Cielo LIO não chegou. O que devo fazer?

Entre em contato com a Central de Atendimento e verifique o status de entrega de sua Cielo LIO.

* 4002 5472 - Todas as localidades
* 0800 570 8472 - Exceto capitais e ligações pelo celular

# Dúvidas Integração Local

## O que eu preciso para colocar meu aplicativo em produção?

Se seu aplicativo já foi certificado, você deve promovê-lo Produção no Dev Console.

A partir desse momento ele estará disponível para todas as LIOs vinculadas à Loja Privada, em caso de Aplicativo Privado; ou em caso de Aplicativo Público ele estará disponível para download na LIO Store.

## Existe algum aplicativo de exemplo disponível?

Disponibilizamos no GitHub um aplicativo Sample de forma que o desenvolvedor consiga ver como funciona as chamadas para utilização do SDK. 

Download do aplicativo Sample: 

> https://github.com/DeveloperCielo/LIO-SDK-Sample-Integracao-Local.

## Preciso me cadastrar para realizar testes?

Sim, é fundamental o cadastro no portal para que você possa obter os tokens de acesso e testar as suas aplicações.

## É necessário colocar todos os itens do pedido na order?

A Cielo LIO funciona com o conceito de Pedido (Order). Assim, o procedimento deve ser sempre o exemplificado no SDK:

1. Criar uma ordem com status draft
2. Adicionar itens à ordem
3. Preparar a ordem para pagamento (place order)
4. Executar o checkout.

<BR>

Se você tem uma variedade de produtos, é interessante criar itens separados para status de relatório na Cielo LIO do lojista.

## Preciso de uma máquina Cielo LIO para realizar os testes de integração local?

Não é necessário ter uma máquina Cielo LIO para realizar os testes.

A Cielo disponibiliza um aplicativo que simula o ambiente da Cielo LIO em qualquer dispositivo Android, permitindo que o desenvolvedor realize os testes nos métodos do SDK e faça o debug da sua aplicação durante o desenvolvimento e a integração com o Cielo LIO Order Manager SDK, sem a necessidade de possuir um hardware da Cielo LIO.

Download do Emulador: 

> https://s3-sa-east-1.amazonaws.com/cielo-lio-store/apps/lio-emulator/1.0.0/lio-emulator.apk