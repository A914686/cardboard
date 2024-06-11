**SDK Cardboard**
=============
Direitos autorais 2019 Google LLC

Este SDK fornece tudo o que você precisa para criar suas próprias experiências de Realidade Virtual (VR) para o Google Cardboard. Ele suporta recursos essenciais de VR, tais como:

 * Rastreamento de movimento
 * Renderização estereoscópica
 * Interação do usuário através do botão do visualizador

Com essas capacidades, você pode construir experiências VR inteiramente novas ou aprimorar
aplicativos existentes com capacidades de VR.

## Comece aqui

Para começar com o SDK Cardboard, veja:

* [Início Rápido para Android NDK](//developers.google.com/cardboard/develop/c/quickstart)
* [Início Rápido para iOS](//developers.google.com/cardboard/develop/ios/quickstart)

## Referência da API

* [Referência da API do SDK Cardboard para Android NDK e iOS](//developers.google.com/cardboard/reference/c)

## Notas de lançamento

As notas de lançamento do SDK estão disponíveis na página de
[lançamentos](//github.com/googlevr/cardboard/releases).

## Roteiro

O roteiro do projeto está disponível na página de
[Projetos](https://github.com/googlevr/cardboard/projects/1).

## Como fazer contribuições

Por favor, leia e siga os passos no arquivo [CONTRIBUTING.md](/CONTRIBUTING.md).

## Licença

Por favor, veja o arquivo [LICENSE](/LICENSE).

## Coleta de Dados

As bibliotecas `cardboard` e `cardboard-xr-plugin` não coletam nenhum dado.
No entanto, quando um código QR é reconhecido durante a varredura conforme solicitado pelo
desenvolvedor, essas bibliotecas podem fazer várias solicitações web para recuperar os
parâmetros do dispositivo visualizador Cardboard.

Especificamente:

*   Se a URL decodificada corresponder a "https://google.com/cardboard" ou
    "https://google.com/cardboard/cfg?p=...", ela é analisada para recuperar os
    parâmetros do dispositivo visualizador Cardboard.
*   Caso contrário, a URL decodificada é solicitada via uma solicitação web normal. Qualquer redirecionamento HTTP é seguido até que uma URL correspondente seja encontrada.

Veja
[QrCodeContentProcessor.java](sdk/qrcode/android/java/com/google/cardboard/sdk/qrcode/QrCodeContentProcessor.java)
(Android) e
[device_params_helper.mm](sdk/qrcode/ios/device_params_helper.mm) (iOS) para o
código que faz o acima.

## Diretrizes de marca

O nome "Google Cardboard" é uma marca registrada de propriedade do Google e não está incluído
nos ativos licenciados sob a Licença Apache 2.0. Cardboard é um SDK de código aberto e gratuito que os desenvolvedores podem usar para criar aplicativos compatíveis
com a plataforma VR do Google Cardboard. Ao mesmo tempo, é importante garantir
que as pessoas não usem a marca "Google Cardboard" de maneiras que possam
criar confusão.

As diretrizes abaixo foram projetadas para esclarecer os usos permitidos da marca "Google
Cardboard".

**Coisas que você pode fazer**:

* Usar a marca "Google Cardboard" para descrever ou referir-se a aplicativos desenvolvidos com
  o SDK Cardboard de maneiras que seriam consideradas "uso justo".
* Usar a marca "Google Cardboard" para fazer declarações factuais verdadeiras sobre
  a compatibilidade ou interoperabilidade do seu aplicativo. Por exemplo, "Este aplicativo é
  compatível com o Google Cardboard" ou "Este aplicativo funciona com o Google Cardboard."

**Coisas que você não pode fazer**:

* Não use a marca "Google Cardboard" de maneira que implique que o Google endossou ou autorizou seu aplicativo ou que faça seu aplicativo parecer ser um produto oficial do Google. Por exemplo, você não deve referenciar seu produto como "um aplicativo oficial do Google Cardboard."
* Não incorpore a marca "Google Cardboard" em seus próprios nomes de produtos,
  nomes de serviços, marcas registradas, logotipos ou nomes de empresas.
* Não exiba a marca "Google Cardboard" de maneira que seja enganosa,
  injusta, difamatória, infratora, caluniosa, depreciativa, obscena ou de outra forma
  objetável para o Google.
* Não altere ou distorça a marca "Google Cardboard". Isso inclui modificar
  a marca através de hifenização, combinação ou abreviação. Por exemplo, não
  diga "G Cardboard" ou "Google-Cardboard."

Além dessas diretrizes, por favor, certifique-se de que você segue as diretrizes de uso de marca registrada disponíveis aqui:
https://www.google.com/permissions/logos-trademarks/.

## Fabricantes
A [especificação do visualizador
Cardboard](https://developers.google.com/cardboard/manufacturers) é
de código aberto e pronta para você começar a construir.
