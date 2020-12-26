# Introdução a React
**Pré-requisitos: Javascript, HTML, CSS** 

## Tópicos 


* [Primeiro APP]()
* [Comandos básicos yarn](comandos_basicos_yarn.md)
* [Componentes](components.md)
* [JSX]()
* [CSS](css.md)
* [Exemplo de .gitignore]()
* [Publicando em uma página no github]()
* [MQTT](mqtt.md)



## Primeiro APP 

Criando o a estrutura incial do aplicativo. 
```
$ npx create-react-app nome-app
```
Será criada uma pasta com nome-app (nome do aplicativo abreviado) contendo os arquivos de uma aplicação simples.   

Para executar esta aplicação entre na pasta e execute o camando: 
``` 
$ yarn start
``` 

### Olá Mundo 

Para criar um olá mundo app serão excluídos todos os arquivos da pasta 'src' e um novo arquivo index.js será implementado. 

Exemplo para o *index.js*: 
```javascript
import ReactDOM from 'react-dom';

ReactDOM.render(
  "Olá Mundo!",
  document.getElementById('root')
);
```

O `ReactDOM` é utilizado para manipular elementos HTML. O `ReactDOM.render` atualizar o elemento HTML de id='root' com o conteúdo "Olá Mundo!". O 'root' é selecionado através de `document.getElementById('root')`. Veja o arquivo 'public/index.html'. 

### Referências
* Curso de React | Rocketseat, https://rocketseat.com.br/starter/curso-gratuito-reactjs
* Curso de React | Curso React + Redux: Fundamentos e 2 Apps do Absoluto ZERO!, https://www.udemy.com/course/react-redux-pt/ 
