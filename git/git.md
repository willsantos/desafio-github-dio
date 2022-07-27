# Git

## Definições

- `HEAD`: Estado atual do nosso código, ou seja, onde o Git nos colocou
- `Working tree`: Local onde os arquivos realmente estão sendo armazenados e editados
- `index`: Local onde o Git armazena o que será *commitado*, ou seja, o local entre a *working tree* e o repositório Git em si.

## Configurações

__Lista as configurações do GIT__
```
git config --global --list
```

__Altera as configurações básicas do usurio GIT__
```
git config --local user.name "Wilson Santos"
git config --local user.email email@example.com
```

## Revertendo um commit antes do Push

__Abre o editor para editar o commit__
```
git commit --amend
```
__Edita a mensagem diretamente__
```
git commit --amend -m"nova mensagem
```
__Retorna os arquivos para o stage__
```
git reset HEAD~1 --soft
```
__Elimina as alterações feitas no stage__
```
git reset HEAD~1 --hard
```

## Salvando para depois
__Salva as alterações atuais para depois__
```
git stash 
```
__Lista os 'save points' do stash__
```
git stash list
```
__Retorna para o stage o 'save point' daquela posição__
```
git stash pop 0 
```
## Alterar a data do commit
```
git commit -m"mensagem do commit"--date="Tue Nov 20 03:00 2018 +0100"
```
## Referencias 
[Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/)