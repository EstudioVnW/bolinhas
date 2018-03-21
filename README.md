# bolinhas

## Passo a passo para gitflow

### 1 - Fazer um fork do repositório no github
Nessa etapa, crie um __fork__ do repositório principal do EstudioVnW. No meu caso, meu fork é https://github.com/julianasobreira/bolinhas-1

### 2 - Clonar no seu computador o seu fork
```
git clone https://github.com/julianasobreira/bolinhas-1 
```

### 3 - Adicionar EstudioVnW como novo remote:
Por padrão, o seu fork estará definido como *origin*. Para adicionar também o EstudioVnW/bolinhas, utilize
 ```
 git remote add estudio https://github.com/EstudioVnW/bolinhas
```
Dessa forma, com 
```
git pull estudio master
```
você irá pegar os dados que estão no repositório do EstudioVnW, e com 
```
git pull origin master
```
pegará os dados no fork

### 4 - Crie um novo arquivo
Vamos criar o arquivo bolinhasBrancas.html. Para isso crie uma nova branch
```
git checkout -b feature-bolinhasBrancas
```
Agora, você estará numa branch (uma nova folha para trabalhar! :) com o nome **feature-bolinhasBrancas** que é igual a branch **master**. Crie seu arquivo aqui. Não esqueça de salvar as alterações
```
git add .
git commit -m "Criei bolinhas brancas"
```

### 5 - Mandar modificações para seu fork
Agora que você terminou a nova feature, é hora de guardá-la no seu repositório remoto.
```
git push origin feature-bolinhasBrancas
```

### 6 - Fazer um pull request
Tá satisfeito com o seu trabalho e quer incluir essa nova feature no repositório do EstudioVnW? É só ir no seu fork no github, selecionar a branch **feature-bolinhasBrancas** e clicar em __New pull request__. Você poderá incluir comentários nessa etapa e escolher para que branch você quer mandar seu pull request. Se você quer mandar para onde todos estão desenvolvendo juntos, manda para **development**.

Agora é só esperar seu pull request ser aceito e sua contribuição no projeto está finalizada!
