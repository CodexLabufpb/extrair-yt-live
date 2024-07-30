# YouTube Live Chat Extractor

Este repositório contém um script Python para extrair mensagens de chat ao vivo do YouTube utilizando a YouTube Data API v3.

## Funcionalidades

- Busca por ID de chat ao vivo de um vídeo específico.
- Coleta de mensagens do chat ao vivo.
- Salvamento contínuo das mensagens em um arquivo CSV.

## Pré-requisitos

Antes de executar o script, você precisa:
- Python 3.x instalado
- Bibliotecas `google-api-python-client` e `pandas` instaladas. Use o comando abaixo para instalar:
  ```bash
  pip install google-api-python-client pandas

## Configuração

- Obtenha uma chave de API do Google Cloud Console habilitada para a YouTube Data API.
- Substitua 'YOUR_API_KEY' pela sua chave de API no script.

## Uso

- Substitua 'VIDEO_ID' no script pelo ID do vídeo do YouTube que possui o chat ao vivo que você deseja extrair.
- Execute o script.
- 
O script continuará rodando e coletando novas mensagens a cada 60 segundos até que seja interrompido manualmente.

## Saída

- As mensagens coletadas serão salvas em um arquivo youtube_live_chat_messages.csv contendo as colunas 'Author' e 'Message'.

## Notas

- Este script apenas coleta mensagens de vídeos que estão atualmente transmitindo ao vivo.
- É necessário monitorar e gerenciar a quota de uso da API para evitar limitações de acesso, a versão grátis tem limite de comentários.
