# Configurações e Comandos

Exercicio 01 - CI|CD - IMPACTA

## Passo a passo - códigos

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


A. No diretorio workspace, criaremos o arquivo.txt
```bash
echo 01 > arquivo.txt
ls
```
![alt text](images/image2.png)


B. Conferindo status e adicionando ao staging
```bash
git status
git add .
git status
```
![alt text](images/image3.png)

C. Commitar o arquivo do staging com a descrição "git add example - arquivo.txt“
```bash
git commit -m "git add example - arquivo.txt"
git status
```
![alt text](images/image4.png)

D. Sobrescrevendo o conteúdo do arquivo.txt:
```bash
echo 02 > arquivo.txt
cat arquivo.txt
```

E. Verificando o diffing no arquivo
```bash
git diff
```
![alt text](images/image5.png)
![alt text](images/image6.png)

F. Adicionado novamente o arquivo no staging e conferir o status
```bash
git add .
git status
```
![alt text](images/image7.png)

G. Verificando o diffing no arquivo
```bash
git diff
```

H. Sobrescrevendo o conteúdo do arquivo.txt:
```bash
echo 03 > arquivo.txt
cat arquivo.txt
```
![alt text](images/image8.png)

I. Verificando o diffing no arquivo
```bash
git diff
```
![alt text](images/image9.png)

J. Fazer o restore do arquivo da área de staging e verificar o status:
```bash
git restore arquivo.txt
git status
```
![alt text](images/image10.png)

K. Realizando o commit do arquivo e verificando o log:
```bash
git commit -m "Segundo Commit - Arquivo.txt"
```
![alt text](images/image11.png)
```bash
git log
```
![alt text](images/image12.png)

L. Adicionando um arquivo gitignore com o seguinte conteúdo: *.txt
```bash
vi .gitignore
cat .gitignore *.txt
```
![alt text](images/image13.png)

M. Criando um arquivo novo.txt e verificar o status:
```bash
echo > novo.txt
ls
git status
```
![alt text](images/image14.png)