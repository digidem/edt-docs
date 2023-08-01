# Serviços

## Syncthing

Uma aplicação de sincronização de arquivos peer-to-peer, gratuita e de código aberto, disponível para a maioria das plataformas. Ela pode sincronizar arquivos entre dispositivos em uma rede local ou entre dispositivos remotos pela internet. A segurança e a integridade dos dados são incorporadas ao design do software. É uma alternativa de código aberto ao [Resilio Sync](https://www.resilio.com).

O aplicativo é usado para manter o conteúdo atualizado (configurações e imagens do mapeo, sites offline, repositório f-droid, etc) disponível quando os dispositivos da comunidade ou da organização estiverem online.

O primeiro handshake entre a instância na nuvem e outros dispositivos é iniciado automaticamente pelo dispositivo EDT Offline, mas precisa ser aceito por alguém com acesso ao serviço de nuvem.

## File Browser

Fornece uma interface de gerenciamento de arquivos dentro de um diretório especificado e pode ser usado para enviar, excluir, visualizar, renomear e editar arquivos. Ele permite a criação de vários usuários e cada usuário pode ter seu próprio diretório. Pode ser usado como um aplicativo independente. É uma alternativa de código aberto ao Google Drive, sem os conjuntos de escritório.\*\*\*\*

É usado para navegar no conteúdo tanto na nuvem quanto no dispositivo offline. A equipe que dá suporte às comunidades deve usá-lo para adicionar ou remover conteúdo hospedado na nuvem. Os dispositivos offline podem usá-lo para compartilhar arquivos com a equipe de suporte ou dentro da rede local.

## Repositório F-Droid

O F-Droid é uma loja de aplicativos e um repositório de software para Android. Os aplicativos podem ser navegados, baixados e instalados pelo aplicativo cliente sem a necessidade de se cadastrar em uma conta. É uma alternativa de código aberto à Google Play Store.

Nós fizemos um fork de um aplicativo cliente e criamos nosso próprio cliente [EDT Apps](https://github.com/digidem/edt-apps), que vem com nosso próprio repositório [EDT app repository](https://github.com/digidem/edt-fdroid-repository), além do repositório que está rodando nos dispositivos EDT Offline.Regular clientes F-Droid também podem usar o repositório EDT adicionando simplesmente a URL à sua lista de repositórios ou escaneando o código QR apresentado.

## Sala Secure Scuttlebut

O aplicativo principal, [Manyverse](https://www.manyver.se/), é uma rede social sem coisas ruins, construída no protocolo SSB ponto a ponto. É gratuito e de código aberto, disponível para desktop e mobile. Não está executando na nuvem de uma empresa, em vez disso, todos os dados vivem completamente nos dispositivos dos usuários. Desta forma, mesmo quando offline, os usuários podem rolar, ler qualquer coisa e até mesmo escrever posts e curtir conteúdo. Quando o dispositivo está de volta online, ele sincroniza as últimas atualizações diretamente com outros dispositivos, através de uma rede Wi-Fi local compartilhada ou na internet.

A Sala SSB é um serviço que permite que pares "se encontrem" online e troquem dados. Ao executar nossa própria Sala, podemos conectar parceiros entre si e também apoiar equipes. Tem recursos de gerenciamento de usuários (listas de permissões e negações + funções de moderador e administrador), tudo administrado através do painel da web.

## Armazenamento Minio

MinIO é uma solução de armazenamento de objetos de alto desempenho que oferece uma API compatível com o Amazon Web Services S3 e suporta todos os recursos principais do S3. É uma alternativa de código aberto ao Amazon S3.

É usado para organizar os dados do Terrastories em buckets. Dessa forma, se um parceiro quiser ter o seu Terrastories publicado na nuvem, podemos sincronizar o bucket do Minio dele, que está sendo executado no dispositivo EDT Offline, e executar uma instância do Terrastories na nuvem puxando esses dados. Isso fornece uma maneira organizada de manter instâncias do Terrastories online e offline em sincronia.