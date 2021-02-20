# nginx-basic
Dois arquivos conf, idiotas, do nginx que eu uso diariamente pra fazer proxy reverso e servir arquivos estáticos;

* Estático: `curl https://raw.githubusercontent.com/pedropalhari/nginx-basic/master/example-page.conf > page.conf`
* Proxy reverso: `curl https://raw.githubusercontent.com/pedropalhari/nginx-basic/master/example-server.conf > server.conf`
* Proxy websocket: `curl https://raw.githubusercontent.com/pedropalhari/nginx-basic/master/example-websocket.conf > websocket.conf`

Ou:

* Estático: `npx degit pedropalhari/nginx-basic/example-page.conf page.conf`
* Proxy reverso: `npx degit pedropalhari/nginx-basic/example-server.conf server.conf`
* Proxy websocket: `npx degit pedropalhari/nginx-basic/example-websocket.conf websocket.conf`

Aproveitando que já estamos aqui:

* Rotear uma porta do servidor para minha máquina `SERVER --> LOCAL`:
* `ssh -R <PORTA_NO_SERVER>:localhost:<PORTA_LOCAL> root@palhari.dev`
* `palhari.dev:<PORTA_NO_SERVER>` agora abre o que roda no meu `localhost:<PORTA_LOCAL>`

* Rotear uma porta da minha máquina para uma do servidor `LOCAL --> SERVER`:
* `ssh -L <PORTA_LOCAL>:localhost:<PORTA_NO_SERVER> root@palhari.dev`
* `localhost:<PORTA_LOCAL>`agora abre o roda no `palhari.dev:<PORTA_NO_SERVER>`
