# Divulgando seu projeto React 

Está página apresenta um pequeno guia de como publicar sua aplicação em uma página do github a partir do seu repositório. 

## Crie o seu repositório 
Pode escolher um nome qualquer.

## Construa seu projeto React 
Use o comando "create-react-app".
Execute o comando `yarn build`.

## Configure o package.json 
`"homepage": "http://seuusuario.github.io/sua_aplicacao"`

Na seção de scripts adicione: 
```
    "predeploy": "yarn build",
    "deploy": "gh-pages -d build",
``` 

## Instale o gh-pages 
`yarn add gh-pages`

## Realize o "Deploy" 
`yarn deploy`

## Configure seu repositório 
Na aba de configurações, vá em "Github Pages", escolha o _branch_ gh-pages e salve.  

## Referências 
* [Utilizando o gh-pages para subir a aplicação React em produção](https://woliveiras.com.br/posts/deploy-de-uma-aplica%C3%A7%C3%A3o-react-no-github-pages/) 
* [Deploy create-react-app project to Github Pages](https://medium.com/@_mariacheline/deploy-create-react-app-project-to-github-pages-2eb6deda5b89)
* [Github Pages](https://pages.github.com/) 
