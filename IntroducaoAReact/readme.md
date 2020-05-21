# Introdução a React
**Pré-requisitos: Javascript, HTML, CSS** 

## Primeiro APP 

Criando o a estrutura incial do aplicativo. 
```
$ npx create-react-app nome-app
```
Será criada uma pasta com nome-app (nome do aplicativo abreviado) contendo os arquivos de uma aplicação simples.   

Para executar esta aplicação entre na pasta e execute o camando: 
``` 
$ npm start
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

#### Trabalhando com JSX

O JSX permite gerar elementos HTMLs a partir de código JavaScript usando uma sintaxe que é JavaScript (JSX) mas muito semelhante ao HTML. Mais informações em https://pt-br.reactjs.org/docs/introducing-jsx.html  

Para usar o JSX é necessário importar o `React`: 
```javascript
import ReactDOM from 'react-dom';
import React from 'react'

ReactDOM.render(
  <div>
    <strong> Olá Mundo! </strong>
  </div>
  ,
  document.getElementById('root')
);
``` 

### CSS 

Será usado o mesmo nome do arquivo a ser aplicado o estilo, neste caso `index.css`. Para este estilor ter efeito é necessário importar o arquivo de estilo no `index.js`: 
```
import './index.css'
```

Exemplo para o arquivo `index.css`:
```css 
body {
    background-color: #222;
    color: #fff 
}
``` 




### Referências
* Curso de React | Rocketseat , https://rocketseat.com.br/starter/curso-gratuito-reactjs
