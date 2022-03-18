# Por que Linux?
<img align="right" alt="engen" width="210" src="https://www.linuxadmingeeks.com/wp-content/uploads/2021/02/cropped-avatar-1295397_640uu3-1.png">

Por que esse carinha é usado em grande escala por diversos servidores, e também, por que na maioria das vezes, as ferramentas para engenharia de dados são desenvolvidas para o sistema operacional Linux. Por isso aprendemos os conceitos Linux.
<br />
<br />
* Aqui você encontrará o conceito e comandos básicos do Linux.
*Lembrando quê: esse estudo é trabalhado no dia-a-dia, sendo um processo orgânico e evolutório, contando com uma linguagem que mescla facilitar a aprendizagem e troca de informações.*
<br />

### CONHECIMENTOS BÁSICOS:
*  O QUE É O LINUX? É um sistema operacional. Mas para não ficar tão vago, vou deixar alguns links que podem te ajudar a conhecer melhor ele.

* [TechTudo - Linux: Tudo o que você precisa saber antes de começar a usar](https://www.techtudo.com.br/noticias/2015/03/linux-tudo-o-que-voce-precisa-saber-antes-de-comecar-usar.ghtml)

<br />

### COMANDOS BÁSICOS DE NAVEGAÇÃO E CONSULTAS NOS DIRETÓRIOS [#verRodando](n)
COMANDOS USADOS NO TERMINAL | O QUE ELE FAZ
----------- | ------
`pwd` | mostra onde estou (na area de trabalho, ou na pasta tal).
`cd NomeOndeQueroIr` | entra nos lugares (entra nas pastas).
`cd ..` | volta para os lugares (retorna para onde você estava).
`cd .` | mostra onde estou (pasta atual).
`cd` | volta para a *HOME*.
`ls` | mostra o que tem no lugar que estou (nome de pastas, documentos, arquivos).
`ls -l` | mostra o que tem no lugar que estou detalhadamente (nome, data, tipo).
`ls -a` | mostra o que tem no lugar que estou detalhadamente inclusive pastas e arquivos ocultos.
`ls/` | mostra todos os arquivos do sistema.
`ls/home` | mostra os arquivos do usuário.
`clear` | limpa a tela do terminal (Ctrl + L, faz a mesma coisa).

* DIRETÓRIO é a mesma coisa que uma pasta (nas antigas, no tempo do [DOS](https://pt.wikipedia.org/wiki/DOS), chamavam as pastas de diretórios).
* PASTA é onde guardamos arquivos e outras pastas.
* ARQUIVO armazena dados, informações. Ex.: um bloco de notas gera um arquivo de texto. Uma foto é um arquivo de imagem.

<br />

### DIRETÓRIOS - CRIAR, RENOMEAR, EXCLUIR E+  [#verRodando](n)
COMANDOS USADOS NO TERMINAL | O QUE ELE FAZ
----------- | ------
`mkdir NomePasta` | cria uma nova pasta.
`cp -r NomePasta NomeDaCopia` | cria uma cópia da pasta.
`rmdir NomePasta` | exclui pasta vazia.
`rm -r NomePasta` | exclui pasta com arquivos dentro.

<br />

### ARQUIVOS - CRIAR, RENOMEAR, EXCLUIR, E+ [#verRodando](n)
COMANDOS USADOS NO TERMINAL | O QUE ELE FAZ
----------- | ------
`echo NomeDocumento` | cria um novo documento.
`mv NomeDocumento NomeNovo` | renomeia o documento.
`cp NomeDocumento NomeDaCopia` | cria uma cópia do documento.
`mv NomeDocumento NomePasta/NomeDocumento` | move o documento para outra pasta
`echo NomeDocumento > NomeDocumento.txt` | transforma o documento criado em um documento na extensão escolhida (no caso do exemplo .txt).
`echo NomeDocumento > NomeDocumento.txt` | usando `>` você sobrescreve dados ao documento.
`echo NomeDocumento >> NomeDocumento.txt` | usando `>>` você acrescenta dados ao documento.
`cat NomeDocumento.txt` | abri o documento e mostra o conteúdo dele.
`cat -n NomeDocumento.txt` | além de abrir o documento e mostrar o conteúdo dele, mostra o número de linhas deste documento.
`rm NomeDocumento` | exclui o documento.

<br />

### .ZIP - COMPACTAR & DESCOMPACTAR ARQUIVOS, E+ [#verRodando](n)
COMANDOS USADOS NO TERMINAL | O QUE ELE FAZ
----------- | ------
`zip Nome.zip NomePasta` | compacta a pasta em um arquivo .zip
`zip -r Nome.zip NomePasta` | compacta a pasta e todos os arquivos que tem dentro dela em um arquivo .zip
`unzip Nome.zip` | descompacta o arquivo .zip
`unzip -l Nome.zip` | me mostra o que tem dentro do arquivo .zip
`unzip -q Nome.zip` | compacta a pasta e não retorna o relatório do que foi compactado.
`touch NomeDocumento` | seleciona apenas o documento especificado

<br />

### .TAR - COMPACTAR & DESCOMPACTAR ARQUIVOS, E+ [#verRodando](n)
COMANDOS USADOS NO TERMINAL | O QUE ELE FAZ
----------- | ------
`tar -cz NomePasta > Nome.tar.gz` | compacta a pasta em um arquivo .tar.gz
`tar -cjf "Nome.tar.gz" "NomePasta/"` | compacta de forma mais leve.
`tar -xz < Nome.tar.gz` | descompacta o arquivo .tar.gz com direcionamento.
`tar -czf Nome.tar.gz NomePasta/` | descompacta o arquivo .tar.gz sem direcionamento.
`tar -xzf < Nome.tar.gz` | descompacta o arquivo .tar.gz sem direcionamento.

* TAR não compacta, ele apenas empacota os arquivos, por isso compactar com ele se torna mais leve. E por ser empacotador que o TAR é usado junto do .gz, que é o compactador real. E o .gz é o formato gerado pelo compactador gzip. Doido né?

<br />

## *DOCUMENTO EM CONSTRUÇÃO*

