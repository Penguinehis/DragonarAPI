# Como Instalar PT-BR <br>
<br>

## Comando de instalação:<br><br>

***wget -qO- https://raw.githubusercontent.com/nvm-sh/nvm/v0.39.0/install.sh | bash && export NVM_DIR="$HOME/.nvm" && [ -s "$NVM_DIR/nvm.sh" ] && . "$NVM_DIR/nvm.sh" && [ -s "$NVM_DIR/bash_completion" ] && . "$NVM_DIR/bash_completion" && nvm install 16 && apt install git screen -y && git clone https://github.com/Penguinehis/DragonarAPI.git && cd DragonarAPI && npm i***

## Comando Iniciar API:<br><br>
<br>

***Subistitua aonde está Chade De ativação pela sua chave, e aonde está Porta pela porta desejada*** 

<br>

***screen -dmS api node DAPIV1.js --token=ChaveDeAtivação --port=Porta***

<br>
Observação a chave de Ativação deve ser adquirida comigo no meu telegram https://t.me/sisudragon , só me enviar uma mensagem para consultar o preço

<br><br>
# Documentação PT-BR <br>
<br>

## 1 - Nucleo checkUser <br>
<br>
Para ser usado o checkuser normal é nescessario o uso de um POST no formato Json, segue o exemplo abaixo: <br><br>

***curl --request POST --url http://127.0.0.1:6888/checkUser --header 'Content-Type: application/json' --data '{ "user": "exemplo"}'***

Tendo como respota a validade do usuario no formato Ymd , segue o exemplo abaixo: <br>

***20220527***

## 2 - Nucleo checkUser2 <br>
<br>
Para ser usado o checkuser 4G é nescessario o uso de um POST no formato Json, segue o exemplo abaixo: <br><br>

***curl --request POST --url http://127.0.0.1:6888/checkUser2 --header 'Content-Type: application/json' --data '{ "user": "exemplo"}'***

Tendo como respota a validade do usuario no formato Ymd , segue o exemplo abaixo: <br>

***{"username":"exemplo","count_connection":"25","expiration_date":"06/04/4760","expiration_days":999982,"limiter_user":"2"}***

## 3 - Nucleo checkOnline <br>
<br>
Para ser usado o checkOnline é nescessario o uso de um GET , segue o exemplo abaixo: <br><br>

***curl --url http://127.0.0.1:6888/checkOnline***

tendo como resposta a quantia online no servidor em formato unico, segue o exemplo abaixo: <br>

***1832***

## 4 - Nucleo servercheck <br>
<br>
Este nucleo é para checkagem da integridade do sistema do API podendendo ser acessado como no exemplo abaixo: <br><br>

***http://127.0.0.1:6888/servercheck***

Ou em caso de ter ativado o HTTPS:<br><br>

***https://127.0.0.1:6888/servercheck***

<br><br><br>

# PENDENTE DE DOCUMENTAÇÃO
## checkUser2 (get), OnlineFULL (get), Gtestuser (Post), gettest (get), getuser (get),
