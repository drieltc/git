# Guia de Git
## 1. Instalando o Git
### Windows
### Linux
### Mac
### Variaveis
## 2. Linkando com o Github
- Criação da chave ssh -> `ssh-keygen -t rsa -b 4096 -C $ghmail`
    - Confirma Y Confirma
    - $ghmail é o e-mail que está cadastrado na conta do github. Uso dessa forma pois, em meu sistema linux, ghmail é uma variável que guarda o meu email.

- Colar a chave SSH no GitHub -> `cat /home/tnb-wsl/.ssh/id_rsa.pub`
    - Imagem print do canto que deve ser colado

- Alias que resolve tudo
```
alias ghssh='ssh-keygen -t rsa -b 4096 -C $ghmail && cat /home/tnb-wsl/.ssh/id_rsa.pub && xclip -sel clip < /home/tnb-wsl/.ssh/id_rsa.pub'

```
- Comando que resolve tudo

```
ssh-keygen -t rsa -b 4096 -C $ghmail && cat /home/tnb-wsl/.ssh/id_rsa.pub && xclip -sel clip < /home/tnb-wsl/.ssh/id_rsa.pub
```

## 3. Comandos
### add
### commit
### status
### log
### push
## 4. Prática 
### 4.x *Branches*
#### 4.x.1 Criando nova *branch*
```
git branch nova_branch
```
O comando acima irá criar auma nova branch, mas você ainda não está trabalhando nela

#### 4.x.1 Mudando para a nova *branch*
```
git checkout nova_branch
```
Agora você já está trabalhando na nova *branch*
