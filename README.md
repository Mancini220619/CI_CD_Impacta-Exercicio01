# Configurações e Comandos

## Passo a passo - codigos

```bash
mkdir Exercicio01
cd Exercicio01/
git init
git config --global user.name "Juliano Mancini"
git config --global user.email "julianomancini@gmail.com"
ls
ls .git/
```
![alt text](images/image.png)


No diretorio workspace, criaremos o arquivo.txt
```bash
echo 01 > arquivo.txt
ls
```
![alt text](images/image2.png)


Conferindo status e adicionando ao staging
```bash
git status
git add .

