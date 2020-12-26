# Trabalhando com JSX

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