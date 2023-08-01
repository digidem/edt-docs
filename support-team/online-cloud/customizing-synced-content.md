# Personalização de conteúdo sincronizado

### 1. Web scraping

A raspagem de sites é feita pelo comando [browsertrix-crawler](https://github.com/webrecorder/browsertrix-crawler) na linha de comando. Encontre mais instruções na [documentação de raspagem](https://www.notion.so/Web-Crawling-c8f980b0fac54cdc9c2d9a308461ddd9).

Algumas experimentações são necessárias para encontrar as melhores práticas sobre como obter exatamente a quantidade de páginas que desejamos raspar e para cada idioma.

A raspagem pode levar muito tempo. Use os arquivos warcz de saída na próxima etapa.

### 2. Carregar para a nuvem

Acesse o serviço do [FileBrowser](https://files.earthdefenderstoolkit.com) na nuvem do EDT.

<figure><img src="../../.gitbook/assets/Untitled.png" alt=""><figcaption></figcaption></figure>

Existem diferentes diretórios dentro do diretório `content`, cada um para um tipo de conteúdo: dados do repositório F-Droid; instaladores para desktop; dados do Mapeo (configurações e tiles); e websites offline.

Crie uma nova pasta para o novo conteúdo, se necessário:

Certifique-se de que há espaço de armazenamento suficiente no servidor e para carregar novo conteúdo basta arrastar para a pasta ou usar o ícone de upload para selecionar o arquivo no seu computador:

<figure><img src="../../.gitbook/assets/Untitled 1 (1).png" alt=""><figcaption></figcaption></figure>

Assim que o novo conteúdo for carregado, podemos sincronizá-lo nos dispositivos do EDT.

### 3. Sincronize

Acesse o serviço [Syncthing](http://sync.earthdefenderstoolkit.com/) na nuvem do EDT e siga os mesmos passos como em [content-syncronization.md](../../device-usage/bundled-applications/content-syncronization.md "menção").

### 4. Adicionar ao dispositivo

Verifique as instruções em [syncing-content.md](../../device-usage/first-steps/syncing-content.md "menção") sobre como começar a sincronizar com um novo dispositivo. Você aprenderá como obter seu ID do Syncthing.

Na instância do EDT Cloud, pesquise por esse ID:

<figure><img src="../../.gitbook/assets/Untitled 6 (1).png" alt=""><figcaption></figcaption></figure>

Dê um nome descritivo ao novo dispositivo e vá para a página de **Compartilhamento**.<figure><img src="../../.gitbook/assets/Untitled 7.png" alt=""><figcaption></figcaption></figure>

Na página **Compartilhamento** selecione todas as pastas relevantes para o novo dispositivo, geralmente as defautls:

<figure><img src="../../.gitbook/assets/Untitled 8 (1).png" alt=""><figcaption></figcaption></figure>

No EDT Cloud você deve ver que o dispositivo está começando a sincronizar:

<figure><img src="../../.gitbook/assets/Untitled 9.png" alt=""><figcaption></figcaption></figure>

Na Offline Toolkit local você também deve ver a sincronização acontecendo com mais detalhes, como taxa de download e quantidade sincronizada até agora.

Pronto. Agora, toda vez que a nuvem atualizar a pasta de conteúdo, os dispositivos Offline Toolkit sincronizarão automaticamente sempre que estiverem online.