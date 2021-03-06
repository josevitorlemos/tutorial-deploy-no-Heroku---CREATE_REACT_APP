<h1 align="center">important!¹ Use todos os comandos dentro da pasta do seu projeto</h1>

<h1 align="center">important!² O seu projeto precisa estar atualizado, na ultima versão presente no GitHub
<br/>
<h1 align="center">
  
 <h3 align="center">!!Siga os passos abaixo e tudo deve funcionar!!</h3>

<h3 align="center">yarn global add heroku || npm install --global heroku</h3>
<p align="center">- Baixar heroku CLI</p>

<h3 align="center">heroku login</h3>
<p align="center">- Autentica sua conta heroku onde irá fazer o deploy</p>

<h3 align="center">heroku create NOME_PROJETO_UNICO --buildpack mars/create-react-app</h3>
<p align="center">- Acesse o link do heroku buildpack para mais informações
<br/>
https://github.com/mars/create-react-app-buildpack <b>ctrl+F: Quick start</b></p>

<h3 align="center">Crie um arquivo chamado <b>static.json</b> na raiz do projeto e adicione as seguintes configurações:</h3>

                            {
                                "root": "build/",
                                "routes": {
                                    "/**": "index.html"
                                }
                            }

<p align="center">"root": Informa ao heroku que a build será executada sempre que iniciar o projeto</p>

<h3 align="center">git remote</h3>
<p align="center">- demonstra todas as branchs do projeto</p>

<h3 align="center">Agora basta fazer o primeiro commit e subir sua aplicação no Heroku</h3>
<p align="center">
# git add --all
<br/>
# git commit -m "deploy projeto"
<br/>
# git push heroku master</p>

<h3 align="center">heroku config:set NODE_MODULES_CACHE=false</h3>
<p align="center">Para desabilitar caches das dependencias e evitar erros.
<br/>
https://devcenter.heroku.com/articles/nodejs-support</p>
    
<h3 align="center">heroku open</h3>
<p align="center">- Irá abrir seu projeto no navegador</p>
