# nginx-basic
Dois arquivos conf, idiotas, do nginx que eu uso diariamente pra fazer proxy reverso e servir arquivos estáticos;

* Estático: `curl https://raw.githubusercontent.com/pedropalhari/nginx-basic/master/example-page.conf > page.conf`
* Proxy reverso: `curl https://raw.githubusercontent.com/pedropalhari/nginx-basic/master/example-server.conf > server.conf`

Ou:

* Estático: `npx degit pedropalhari/nginx-basic/example-page.conf page.conf`
* Proxy reverso: `npx degit pedropalhari/nginx-basic/example-server.conf server.conf`

Aproveitando que já estamos aqui:

* Rotear uma porta do servidor para mim:
* `ssh -R 5050:localhost:5050 root@palhari.dev`
* palhari.dev:5050 agora abre o que roda no meu localhost:5050

* Rotear uma porta do minha para um servidor:
* `ssh -L 5050:localhost:5050 root@palhari.dev`
* localhost:5050 agora abre o roda no palhari.dev:5050
