## **CONCEITO**

## GIT:   

Sistema de versionamento de códigos distribuídos. Além de ser um sistema distribuído, ele foi projetado com desempenho, segurança e flexibilidade. Ele soluciona, monitora e ajuda a criar diferentes versões de nosso código, dentro da nossa máquina.

## GITHUB:

É o repositório online, onde serão armazenados nossos códigos. Ele hospeda o repositório principal, do qual os colaboradores podem fazer cópias para seus próprios trabalhos. É um repositório remoto, logo, todos os arquivos são comitados.

:warning: Apesar de serem diferentes, são tecnologias complementares !! 





#### CONTEÚDO

**Sha1:** Algoritmo de encriptação. A encriptação gera um conjunto de caracteres de identificação de 40 dígitos, sendo único e serve como forma de identificação.

⚠️ Cada mudança, gera uma chave nova, se desfizer a mudança, volta a chave anterior.

**São três tipos básicos de objetos do Git:**

·     Blobs (Blocos básico de composição): contém o tipo do objeto; tamanho do arquivo; \0;e o conteúdo do arquivo; contém metadados.

·     Trees (Árvore): Armazenando e apontando para tipos de blobs diferentes e aponta para outras arvores; também contém sha1 desses metadados;

·     Commits: Contém todas as informações, contém autor, mensagem, timestomp; aponta para arvores e parentes.

É um ciclo, se o Sha1 de um blobs for alterado, logo. o Sha1 das Trees e Commits também serão alterados.

**Ciclo de vida do arquivo:**

Untracked: São os arquivos que o Git ainda não tem ciência, são podem ser rastreados;

Tracked: subdivide em

·     Unmodified: Arquivos que não foram modificados; (se remover, se torna untracked/)

·     Modified: Arquivos que já sofreram modificações;

·     Staged: Arquivos em preparação para ser parte de um commit.

Há uma transitoriedade, quando edita um arquivo ele se torna um Staged e ao realizar o comando Commit, eles deixam de ser Staged e passam a ser um arquivo Unmodified, pois já realizou o Snap Shot (criação de uma foto) uma vez que já acabou todas as alterações do arquivo. Permitindo assim que se inicie um novo ciclo.

**Há dois ambientes:**

·     Ambiente de desenvolvimento:

o  Working Directory

o  Staging Area

o  Local Repository

·     Servidor: Remote Repository

Quando ocorre um Commit, esse arquivo passa a integrar o seu repositório local e este por sua vez, pode ser empurrado para um repositório remoto.

⚠️ Repositório remoto, só recebe um arquivo comitado, se não estiverem não conseguem ser enviados para um repositório remoto.

 

#### Comandos importantes para Windows 

CMD - "PROMPT DE COMANDO": 

·     CD: Navegar entre as pastas;

·     DIR: Listar diretório de pastas;

·     MKDIR: Criar uma nova pasta (mkdir + nome para pasta)

·     DEL: Aplicando o del, removerá apenas os arquivos contido dentro;

·     RMDIR: Removerá pasta completa;

·     CD .. :Retroceder um nível de navegação;

·     CLS: Limpar Terminal;

GIT

·     Git init: comando que inicializa/cria um repositóri;

·     Git add: move o arquivo untracked para staged;

·     Git add *: Arquivo que esta modificado/ tudo presente do diretório de trabalho e add para staged;

·     Git commit -m "Adicionar aqui mensagem": Para Comitar/ Guardar em um repositório local/mover toda a area staging para o repositório local;

·     Git config -- list: lista de todas as configurações do seu GIT;

·     Git config -- global -- unset user.email: remover o email cadastrado;

·     Git config -- global -- unset user.name: remover o nome(usuário) cadastrado;

·     Git config -- global -- user.email "digitar email/preferencialmente o cadastrado no Github";

·     Git config -- global -- user.name "digitar usuário/preferencialmente o cadastrado no Github";

·     Mv "nome arquivo": mover o arquivo;

·     Git status: Ajuda a monitorar o status do arquivo, aqui dirá se arquivo é Untracked, Unmodified, Modified, Sraged (Conceito e mudanças em "conteúdo importante");

·     Ls -A: Mostrar repositório Oculto;

·     Git remote add origin (copiar o link do Github do repositório)

·     Git remote -v: Mostrará as listas de repositórios remotos cadastrados por mim;

·     Git push origin master: Empurrar o conteúdo para Github;

·     Git pull origin master: Puxar o conteúdo para a maquina;

·     Git Clone: Clonar um repositório. 



#### Possibilidade de Conflitos:

Quando ocorre mais de uma alteração em uma mesma linha, pode ocorrer um conflito, um erro, logo quando for empurrar para o repositório remoto dará errado, pois terá já terá um código mais atualizado e o seu desatualizado.

Ideal é que faça:

Puxar (Git pull origin master) o código, fazer as alterações necessárias para integrar e somente após isso empurrar novamente para o repositório remoto (Git push origin master).

Lembre-se do Git commit - m "resolver conflitos" antes de empurrar para o repositório remoto.

 

### Download Windows 💻

Para Download do Git, versão atualizada, acessar o site: https://git-scm.com/download/win;



##### GitHub

É necessário o acesso ao site [GitHub](https://github.com/) e realizar o cadastro, para conseguir criar o repositório e fazer a comunicação entre a máquina e o repositório remoto.

 