# Recursos WEB

## Rodando a aplicação no servidor de produção 

Instalação do gerenciador de aplicações 
```
npm install -g pm2
```

Iniciar
```
pm2 start nome_do_arquivo.js --name=MeuAplicativo
```

Verificar o status 
```
pm2 status
```

Reiniciar
```
pm2 restart MeuAplicativo
```

Parar
```
pm2 stop MeuAplicativo 
```

Deixar de gerenciar 
```
pm2 delete MeuAplicativo 
```

## Referências 

1. PM2, http://pm2.keymetrics.io 
