---
layout: post
title: Sensores e dados
category: posts
---

Um dos pontos essenciais para a construção de soluções IoT é observarmos e sentirmos o mundo externo. Para tal, utilizamos sensores.

No hackathon, teremos alguns sensores, e podemo emular ou simular outros também. Abaixo vão as ideias que trouxemos como pontapé inicial:

**Utilizando o nosso próprio smartphone**. O smartphone tem vários sensores como gps, giroscópio, luminosidade, nível de sinal, nível de bateria, etc. Existem aplicativos como o Automate (https://llamalab.com/automate/) que permite construirmos rotinas de leituras dos sensores muito rapidamente e utilizando um plugin de MQTT (https://github.com/nosybore/Tasker-MQTT-Publish-Plugin), que é um protocolo para IoT, conseguimos facilmente enviar os dados para a plataforma dojot.

Existe **emulador do Sense Hat Raspberry Pi** (https://www.raspberrypi.org/blog/desktop-sense-hat-emulator/), que é uma placa utilizada em concursos como Astro-Pi (https://astro-pi.org/). O Sense Hat tem sensores de temperatura, pressão, giroscópio, acelerômetro, Matriz de Led, joystick. Um código de referência para integração com a dojot está disponível em: https://github.com/rascaraficci/dojot-sense-hat.

No github da dojot está disponível um [**emulador de dispositivos MQTT**](https://github.com/dojot/mqtt-emulator) que pode ser configurado para gerar dados de sensores.

Para o Hackathon teremos disponíveis **Beacons da Taggen**. Os beacons são dispositivos que permitem, entre outras coisas, que outros dispositivos reconheçam que estão fisicamente proximos de outro dispositivo ou de um local ([Mais informações](
https://developers.google.com/beacons/)).

Esses sensores precisam de um gateway para conectá-los a dojot. A sugestão de gateway é utilizar o próprio smartphone com o [aplicativo Beacon Scanner](https://github.com/Bridouille/android-beacon-scanner). A Taggen desenvolveu em Xamarin [um gateway mobile](https://github.com/taggensistemas) que detecta beacons, pega a posição gps e envia esses dados para o dojot. Podemos alterar esse app, por exemplo.
