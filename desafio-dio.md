# Desafio Dio Primeiro Repositório :satisfied:

Este repositório serve como uma forma teste para guardar anotações realizadas na aula de Git/Github



## GIT E GITHUB :cloud:

Git é uma ferramenta de versionamento de código que foi criada em 2005 por Linus Torvalds; 

Surgiu como uma necessidade de edição e manutenção de código realizada por várias pessoas ao mesmo tempo e também para o armazenamento desses códigos. 

Github é o lugar de armazenamento de código, construído pela Microsoft. 

Há outras tecnologias similares ao Github, como gitbucket e gitlab. 

GIT é um programa comun line interface, não tendo interface gráfica. 

Há diferenças de comandos entre windows e linux. 

Comandos windows 

Dir - lista todas as pastas e diretórios que estão à volta da pasta de acesso. (no linux é LS). 

cd (change diretory) -serve para mudar o diretório --> ex: cd /windows (após digitar esses comandos, e colocar dir, ele dará outros diretórios relacionados à pasta windows).. 

para voltar, basta digitar cd .. (para retroceder um nível). 

cls - clear screen (limpa a tela) --> linux é clear. 

a tecla tab completa nomes da pasta em que está no termina. (ex: win (tab) ele completa). 

para criar uma pasta, usa-se mkdir (make diretory) + nome da pasta. 

echo retorna um valor --> echo hello > hello.txt (aqui o > significa output, e irá criar um arquivo chamado hello em txt caso não haja nenhuma já criada). 

No windows há uma diferença entre deletar arquivos e deletar repositórios. 

o comando del serve para deletar apenas arquivos e não pastas. Se usado para deletar uma pasta, ele irá deletar os arquivos desta pasta, mas ela continuará existindo. 

Para remover uma pasta, usa-se rmdir (remove directory). --> rmdir nomedapasta /s /q 

 

Entendendo como o git funciona 

SHA1 - segure hash algorithm --> ele irá encriptar o algoritmo de forma segura a cada alteração do código. 

com o bash aberto, --> openssl sha1 nomedoarquivo.text ele irá mostrar a chave gerada para aquele estado do arquivo. Se algo for alterado, como uma simples vírgula, ele gerara uma outra chave de 40 caracteres como criptografia. 

Objetos internos no git --> 

Objetos básicos do git: 

O git irá guardar os objetos e gerar metadados destes objetos. Tais objetos são guardados dentro do BLOB. 

BLOBS- contém metadados do arquivo. Ele irá possuir o tipo do objeto, o tamanho do objeto, \0, a chave do arquivo. Essa é a estrutura básica de um blob. Ele não guarda o nome do arquivo em si. 

TREES - Armazenam BLOBS diferentes e commits. Ela possui o tamanho, a \0, o blob, o sha1 e o nome do arquivo. Ela pode apontar para outras árvores. Elas também possuem o sha1 dos metadados das árvores. Se mudar um arquivo, como do blob, irá mudar a estrutura da árvore. 
