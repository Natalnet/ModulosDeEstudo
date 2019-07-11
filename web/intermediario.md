# Recursos WEB

## Rodando a aplicação no servidor de produção 

Instalação do gerenciador de aplicações 
```
$ npm install -g pm2
```

Iniciar
```
$ pm2 start nome_do_arquivo.js --name=MeuAplicativo
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

Executar em uma porta desejada 
```
pm2 start binary-file -- --port 1520
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

Para verificar se existe algum erro de escrita nos arquivos de configurações 
```
$ sudo nginx -t
```

### Servindo uma página estática

Crie o diretório paras os arquivos da página 
```
$ sudo mkdir -p /var/www/test.com/html
``` 

Verifique as permissões de acesso a este diretório

Crie uma página simples
``` 
$ nano /var/www/test.com/html/index.html
``` 
Exemplo de conteúdo para index.html 
```html 
<html>
    <head>
        <title>Bem vindo à test.com!</title>
    </head>
    <body>
        <h1> Página test.com funcionando! </h1>
    </body>
</html>
``` 

Editando o arquivo de configuração para a página no Nginx 
```
$ sudo nano /etc/nginx/sites-available/teste.com
``` 

Exemplo de configuração para 'teste.com' 
```
server {
        listen 80;
        listen [::]:80;

        root /var/www/teste.com/html;
        index index.html index.htm index.nginx-debian.html;

        server_name teste.com www.teste.com;

        location / {
                try_files $uri $uri/ =404;
        }
}
```

Crie um link simbólico para os sites habiltados no Nginx 
```
$ sudo ln -s /etc/nginx/sites-available/teste.com /etc/nginx/sites-enabled/
```

Faça a checagem de sintaxe
```
$ sudo nginx -t
```

Reinicie o Nginx
```
$ sudo systemctl restart nginx
``` 
### Servindo uma aplicação react 

Gerando o código de produção 
```
$ yarn build 
``` 
Semelhante a seção anterior, mas os arquivos do servidor web estão na pasta build. 



## Referências 

1. PM2, http://pm2.keymetrics.io 
1. How To Install Nginx on Ubuntu 16.04, https://www.digitalocean.com/community/tutorials/how-to-install-nginx-on-ubuntu-16-04
1. How To Set Up a Node.js Application for Production on Ubuntu 16.04, https://www.digitalocean.com/community/tutorials/how-to-set-up-a-node-js-application-for-production-on-ubuntu-16-04
1. A guide to hosting static websites using NGINX, https://medium.com/@jgefroh/a-guide-to-using-nginx-for-static-websites-d96a9d034940
1. How To Set Up Nginx Server Blocks (Virtual Hosts) on Ubuntu 16.04, https://www.digitalocean.com/community/tutorials/how-to-set-up-nginx-server-blocks-virtual-hosts-on-ubuntu-16-04  
1. Como Instalar o Nginx no Ubuntu 16.04,  https://www.digitalocean.com/community/tutorials/como-instalar-o-nginx-no-ubuntu-16-04-pt
1. How to Configure NGINX, https://www.linode.com/docs/web-servers/nginx/how-to-configure-nginx/
