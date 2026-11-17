# EkballoDeck

O EkballoDeck é um fork do [PhoneBox, de Ersin KOÇ](https://github.com/ersinkoc/phonebox). Ele transforma um celular Android em um painel de controle por toque no estilo Stream Deck para **OBS Studio**, automações e dashboards.

- **OBS Studio** — alterne cenas, controle fontes e áudio e acione gravação ou transmissão pelo painel.
- **Automações** — acione atalhos, macros, scripts e webhooks ou controle dispositivos pelo Home Assistant.
- **Dashboards** — monte páginas com dados do computador, mídia e outras informações usando o editor visual. O catálogo herdado tem **120 widgets** e **30 templates**.

## Como experimentar

O aplicativo Android se conecta a um agente em execução no Windows, no macOS ou no Linux, por USB com ADB ou por Wi-Fi com pareamento. Funciona sem root e sem alterar a ROM.

1. Compile o APK de depuração e execute o agente a partir deste código-fonte. O [guia de desenvolvimento](docs/DEVELOPMENT.md) traz os pré-requisitos e os comandos para cada sistema.
2. Instale o APK local no Android e conecte o telefone. Consulte o [guia de conexão](docs/SETUP.md) para USB e Wi-Fi.
3. Abra as configurações do agente no computador. Em **Integrations**, configure o OBS WebSocket. Em **Pages**, adicione os controles do OBS ou escolha um template de **Control Deck**. Habilite a opção de controle no widget do OBS. Veja o [guia de controles](docs/CONTROL-DECK.md).

Esta branch traz o primeiro rebranding, com o nome EkballoDeck no Android e na interface do agente e um ícone provisório no Android. Os instaladores e a atualização integrada ainda apontam para o PhoneBox original. Para testar o EkballoDeck, use os artefatos compilados a partir desta branch e desative **Install new releases automatically** na seção **Updates** do agente.

## Licença

O projeto mantém a [licença MIT](LICENSE) e o aviso de copyright do PhoneBox.
