# Componentes 

## Componente Simples 

Exemplo de um componente extremamente simples sem uso de estruturas JSX.  
```javascript 
export default function Simples() {
    return  "Componente Simples!"
}
``` 

Para incluir este componente, basta indicar o nome do componente e sua localização: 
```javascript
import Simples from './componentes/Simples'
```

Para chamar o componente, basta usar a sintaxe JSX:
```javascript
<Simples></Simples>
```

## Parâmetros 

Ao chamar um componente é possível passar parâmentros para este componente e a forma de utilização é muito semelhante ao uso de atributos na linguagem HTML. 

O código a seguir mostra um componente com dois atributos `p1` e `p2` sendo utilizados. 
```javascript 
import React from 'react' 

export default function Parametro(props) {
    return (
        <div> 
            <h2> Com Parametro </h2>
            <p> 
                <strong> {props.p1} </strong> e <strong> {props.p2} </strong>     
            </p> 
        </div>
    );
}
``` 
Note que props.p1 está envolvido por `{ }` permitindo que props.p1 seja interpretado recuperando o conteúdo de p1.  

O conteúdo destes parâmetros é definindo na chamada do componente como mostra o código abaixo: 
```javascript

import './index.css'
import ReactDOM from 'react-dom';
import React from 'react'

import Parametro from './Componentes/Parametro'

ReactDOM.render(
  <div>
    <Parametro p1="Primeiro" p2="Segundo"></Parametro>
  </div>
  ,
  document.getElementById('root')
);
```

O resultado em um navegador de internet fica semelhante a figura abaixo: 


![Tela do Navegador](com_parametro.png)