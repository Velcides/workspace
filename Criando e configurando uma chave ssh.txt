# Criando e configurando uma chave ssh
-Gera a chave pro email
$ ssh-keygen -t ed25519 -C velcidesufpa@gmail.com

-Acessando a chave e copiando para adicionar no github
$ cd /c/Users/pitag/.ssh
$ cat id_ed25519.pub
copiar e colar a chave gerada

-Adiciona a chave ssh no seu computador
$ eval $(ssh-agent -s)
$ ssh-add id_ed25519

Ao usar o git clone selecionar o link na aba SSH.

Comandos do git:
Ininciando o repositório localmente:

git init - inicia o repositório
para visualizar repositório vazio ls -a

# Configuração inicial
git config --global user.email "email"
git config --global user.name Velcides
git config --global --unset user.name - remove

git add - adiciona arquivo para commit
git add * adiciona todas as modificações
git add. 

git commit -m ""

git status - verifica alteração nos arquivos do repositório

Acessando o repositório remoto

git remote add origin - "empurra" para um repositório remoto o nosso repositório local
git remote -v - lista repositórios remotos cadastrados
git push origin master - "empurra" as modificações pro repositório remoto
git pull origin master - atualiza seus arquivos, ideal faze-lo antes do push

## Links 
[Sintaxe Básica Markdown](https://www.markdownguide.org/basic-syntax/)
