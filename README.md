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
git status
```
![alt text](images/image3.png)

Commitar o arquivo do staging com a descrição "git add example - arquivo.txt“
```bash
git commit -m "git add example - arquivo.txt"
git status
```
![alt text](images/image4.png)

Sobrescrevendo o conteúdo do arquivo.txt:
```bash
echo 02 > arquivo.txt
cat arquivo.txt
```

Verificando o diffing no arquivo
```bash
git diff
```
![alt text](images/image5.png)
![alt text](images/image6.png)

Adicionado novamente o arquivo no staging e conferir o status
```bash
git add .
git status
```