# Projeto para estilização de páginas utilizando SASS
O projeto consiste em um script Node.js que permite ao usuário passar um arquivo ou uma pasta como parâmetro. O script lerá os arquivos com a extensão .md dentro da pasta especificada ou o arquivo individual fornecido pelo usuário. Em seguida, usa expressões regulares (regex) para extrair os links contidos nos arquivos Markdown.

Passos do Projeto:

1. Criar arquivo SASS.
2. Utilizar terminal para que crie arquivos CSS baseados nos arquivos SCSS.
3. Utilizar import dentro do SCSS de forma que unifique diversos arquivos.
4. Utilizar variaveis.

## Instalando SASS

Dentro do terminal execute o comando abaixo, certifique-se de ter instalado o npm em sua maquina.

**Instalando:** npm install sass

## Criando arquivo SASS
Os arquivos tem que possuir a extensão *.sass, os codigos de para estilização são os mesmo utilizados para as páginas CSS.

No nosso exemplo criamos 2 arquivos resete.scss e estilo.scss

A partir desses arquivos são criados os arquivos CSS para serem utilizados em nossas páginas, para isso podemos utilizar alguns comando dentro do terminal.

1. **Criar arquivo por arquivo**: sass .\_cdn\scss\estilo.scss .\_cdn\css\estilo.css 
2. **Criar/Atualiza todos arquivos de uma pasta**: sass .\_cdn\scss\:.\_cdn\css\
3. **Fica monitorando a pasta e após salvar cria/atualiza o arquivo**: sass .\_cdn\scss\:.\_cdn\css\ --watch
4. **Fica monitorando a pasta e após salvar cria/atualiza o arquivo  minificado**: sass .\_cdn\scss\:.\_cdn\css\ --watch --style=compressed

## Separando arquivos e usando @import
Para uma melhor visualização e para manter o código mais organizado podemos utilizar o comoando @import dentro do arquivo SCSS para que ele importe dados de outro arquivo, os arquivos que serão importandos dentro do nosso @importe devem contes no inicio do nome o "_", dessa forma caso esteje utilizando o comando que fica monitorando e gerando os arquivos CSS automaticamente não crie esses arquivos uma vez que serão importandos dentro de outro.