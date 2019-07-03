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
$ pm2 status
```

Reiniciar
```
$ pm2 restart MeuAplicativo
```

Parar
```
$ pm2 stop MeuAplicativo 
```

Deixar de gerenciar 
```
$ pm2 delete MeuAplicativo 
```

## Nginx web server 

Parar o servidor:
```
$ sudo systemctl stop nginx
```

Iniciar:
```
$ sudo systemctl start nginx
```

Reiniciar: 
```
$ sudo systemctl restart nginx
```

Recarregar: 
```
$ sudo systemctl reload nginx
```

Para habiltar que o serviço inicie automaticamente quando o servidor for reiniciado: 
```
$ sudo systemctl enable nginx
```

## Referências 

1. PM2, http://pm2.keymetrics.io 
1. How To Install Nginx on Ubuntu 16.04, https://www.digitalocean.com/community/tutorials/how-to-install-nginx-on-ubuntu-16-04
1. How To Set Up a Node.js Application for Production on Ubuntu 16.04, https://www.digitalocean.com/community/tutorials/how-to-set-up-a-node-js-application-for-production-on-ubuntu-16-04
