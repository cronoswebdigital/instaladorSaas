PROCESSO DE INSTALAÇÃO DO PAINEL MULTI-ATENDIMENTO

Obs:. Caso você não consiga fazer a instalação do painel, nós cobramos 119,85 Reais para fazer para você a instalação e deixar pronto para uso.
Para mais detalhes, por favor, nos mande mensagem para (32) 9 9871-9354
Nosso suporte funciona de segunda a sábado, de 15 ás 19 horas. 


-------------------------------------------------------------------------------------------------------------------------------------------------------
INICIO DA INSTALAÇÃO

ATENÇÃO:>>>
SUGERIMOS QUE VEJA TODO O VIDEO PRIMEIRAMENTE, ANTES DE INICIAR A INSTALAÇÃO, 
PARA VOCE FICAR FAMILIARIZADO COM OS PROCEDIMENTOS.

CONTRATE UM DOMINIO COM UMA HOSPEDAGEM.
SUGERIMOS A HOSGATOR.

Sites que serão usados  (gerados na Cloudflare)
https://nome-do-site-para-o-backend.SEUDOMINIO.com.br
https://nome-do-site-para-o-frontend.SEUDOMINIO.com.br

CONTRATE A VPS HETZNER. PODE SER O SERVIDOR VPS MAIS BARATO
SISTEMA OPERACIONAL UBUNTU 20.04 LTS

VA NO SITE CLOUDFLARE E FAÇA UMA CONTA (GRATIS) 

APONTE A CLOUDFLARE PARA O SEU SITE. (NO VIDEO TEM ESSA PARTE ENSINANDO)
Para essa configuração voce precisará do IP da sua VPS Hetzner

No windows, instale o programa Bitvise SSH (incluido nos arquivos)

Entre no programa Bitvise SSH e no campo "Host" digite o IP do seu servidor VPS.
Em "Port" digite o numero 22
No campo "username" digite root
Em "Initial method" selecione "password"
Selecione a caixa "Store encrypted password in profile"
Em "password" digite a senha do seu servidor VPS (GERALMENTE E ENVIADA POR EMAIL)
Selecione a caixa "Enable password over kbdi fallback"
Em "elevation" marque a caixa "Default"
Clique em login
CLIQUE EM "ACEPT AND SAVE"

AGORA NO PROGRAMA BITVISE APARECEU O ICONE "NEW TERMINAL"
CLIQUE NO BOTAO "NEW TERMINAL CONSOLE"
SELECIONE E COPIE (TECLA "Ctrl" + A TECLA "C") A SENHA DO SERVIDOR (GERALMENTE E ENVIADA POR EMAIL)
DENTRO DO TERMINAL DE UM CLIQUE COM O MOUSE NO BOTAO DIREITO E APERTE A TECLA "ENTER"
A SENHA NAO VAI APARECER NO TERMINAL, ISSO E NORMAL
NESSE MOMENTO VA NA CONFIGURAÇÃO DO SEU SERVIDOR, 
CLIQUE EM "RESCUE" APOS ISSO CLIQUE EM "RESET ROOT PASSWORD"
CLIQUE NOVAMENTE EM "RESET ROOT PASSWORD"
DE UM CLIQUE EM CIMA DA SENHA QUE ELA JA E COPIADA AUTOMATICAMENTE
APOS ISSO DE UM CLIQUE COM O BOTAO DIREITO DO MOUSE E APERTE A TECLA "ENTER"
CLIQUE NOVAMENTE COM O BOTAO DIREITO DO MOUSE E APERTE A TECLA "ENTER"
NESSE MOMENTO O TERMINAL E DESCONECTADO
VOLTA AO PROGRAMA BITVISE E NA CAIXA "PASSWORD" COLE A SENHA E CLIQUE EM "LOG OUT"
CLIQUE EM "LOGIN"
CLIQUE EM "NEM TERMINAL CONSOLE"

ATENÇAO:>>>
OBS, SE POR ACASO REAPARECER UMA CAIXA (POP PUP) PEDINDO OUTRA SENHA, ENTRE NA CONFIGURAÇÃO DO SEU SERVIDOR, 
CLIQUE EM "RESCUE" APOS ISSO CLIQUE EM "RESET ROOT PASSWORD"
CLIQUE NOVAMENTE EM "RESET ROOT PASSWORD"
DE UM CLIQUE EM CIMA DA SENHA QUE ELA JA E COPIADA AUTOMATICAMENTE
COLE A SENHA COPIADA DENTRO DA PAGINA (POP PUP) QUE APARECEU

---------------------------------------------------------------------------------------------------------------------------------------------------

SELECIONE E COPIE (TECLA "Ctrl" + A TECLA "C") O CODIGO ABAIXO E NO TERMINAL DE UM CLIQUE COM O BOTAO DIREITO QUE O CODIGO JA APARECE NO TERMINAL, APOS ISSO APERTE A TECLA "ENTER"

sudo apt-get update && sudo apt-get upgrade -y

----------------

SELECIONE E COPIE (TECLA "Ctrl" + A TECLA "C") O CODIGO ABAIXO E NO TERMINAL DE UM CLIQUE COM O BOTAO DIREITO QUE O CODIGO JA APARECE NO TERMINAL, APOS ISSO APERTE A TECLA "ENTER"

sudo apt install -y git && git clone https://github.com/cronoswebdigital/instaladorSaas.git install_whaticket && sudo chmod -R 777 install_whaticket  && cd install_whaticket  && sudo ./install_primaria

----------------
DIGITE
0
APERTE A TECLA "ENTER"

DIGITE a senha DEPLOY
95135789
aperte a tecla "enter"

DIGITE
https://github.com/cronoswebdigital/saasWhaticket.git
aperte a tecla "enter"

DIGITE
empresa02
aperte a tecla "enter"

DIGITE
9999
aperte a tecla "enter"

DIGITE
9999
aperte a tecla "enter"

DIGITE o link para o frontend feito na cloudflare
https://nome-do-site-para-o-frontend.SEUDOMINIO.com.br
aperte a tecla "enter"

DIGITE o link para o backend feito na cloudflare
https://nome-do-site-para-o-backend.SEUDOMINIO.com.br
aperte a tecla "enter"

DIGITE
3001
aperte a tecla "enter"

DIGITE
4001
aperte a tecla "enter"

DIGITE
5001
aperte a tecla "enter"

username:DIGITE
oieeteckmark
aperte a tecla "enter"

passowrd
Tokem:
Solicite o "token" de acesso atraves do whatsapp (32) 9 9871-9354
Nosso horario de atendimento e das 15 ás 19 horas, de segunda a sabado.
SELECIONE E COPIE (TECLA "Ctrl" + A TECLA "C") o "TOKEN"
DENTRO DO TERMINAL DE UM CLIQUE COM O MOUSE NO BOTAO DIREITO E APERTE A TECLA "ENTER"
A SENHA NAO VAI APARECER NO TERMINAL, ISSO E NORMAL


Tokem: xxxxxxxxxxxxxxxxxxxx
xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx

DIGITE
cd /home/deploy/sacmais/backend

DIGITE
npm i @whiskeysockets/baileys

DIGITE
npm install @adiwajshing/keyed-db@0.2.4


Continuando...

Copie para a sua area de trabalho, a pasta "lib" que foi enviado junto com os arquivos do painel.

Abra o "bitvise, apos isso abra o painel  "New SFTP window"
EM "Remote files" digite o "endereço" no campo a baixo.

/home/deploy/sacmais/backend/node_modules/@adiwajshing/baileys/lib
APERTE ENTER

Apague todos os arquivos que estao dentro da pasta "lib", que esta do lado direito do painel
De 2 cliques na pasta "lib" que esta na sua area de trabalho ao lado esquerdo do painel.
Selecione todos os arquivos da pasta "lib" e arraste para o lado, para serem copiadas para dentro da pasta "lib" do lado direito

FECHE O PAINEL "New SFTP window"

Continuando....
---------------------------------------------------------------------------------------------------
---------------------------------------------------------------------------------------------------
Caso NÃO tenha feito o cadastro no Gerecianet,
pule essa parte, e va direto para >>>>> ATUALIZAÇÃO DO PAINEL <<<<<< LOGO ABAIXO
---------------------------------------------------------------------------------------------------
---------------------------------------------------------------------------------------------------
Se você fez o cadastro na Gerecianet, CONTINUE POR AQUI...
Copie para a sua area de trabalho, o certificado da Gerecianet.
(caso nao tenha feito ainda a sua conta na Gerecianet, Nao tem problema.
Esse processo podera ser feito posteriormente.)
Caso nao tenha feito o cadastro no Gerecianet.
Pule essa parte e va direto para >>>>> ATUALIZAÇÃO DO PAINEL <<<<<< LOGO ABAIXO

INTEGRANDO O GATEWAY DE PAGAMENTO GERECIANET
Copie o arquivo do certificado feito na gerecianet e cole na area de tabalho

NO PAINEL DO PROGRAMA BITVISE CLIQUE EM "New SFTP window"

Em "Remote files" no campo abaixo digite
/home/deploy/sacmais/backend/certs
Certifique-se que o desktop do seu computador/notebook esteja aparecendo na parte esquerda do painel New SFTP windows,
apos isso selecione e "arraste" o arquivo do certificado para a direita do painel.
O arquivo do certificado tem que esta dentro da pasta "certs"

Prosseguindo...
Em "Remote files" no campo abaixo digite
/home/deploy/sacmais/backend/

De dois cliques no arquivo ".env" para abri o arquivo e cole os SEUS CODIGO SUBSTITUINDO OS CODIGO DO PAINEL 

GERENCIANET_SANDBOX=false
GERENCIANET_CLIENT_ID=Client_Id_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
GERENCIANET_CLIENT_SECRET=Client_Secret_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
GERENCIANET_PIX_CERT=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx
GERENCIANET_PIX_KEY=xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx

salve o arquivo
feche o painel
"New SFTP window"

---------------------------------------------------------------------------------------------------
---------------------------------------------------------------------------------------------------
---------------------------------------------------------------------------------------------------
>>>>> ATUALIZAÇÃO DO PAINEL <<<<<<

No terminal DO PROGRAMA BITVISE
digite os comandos abaixo

DIGITE
cd /home/deploy/sacmais/
aperte a tecla "enter"

DIGITE
chmod +x ./update
aperte a tecla "enter"

DIGITE
./update
aperte a tecla "enter"

DIGITE
sudo systemctl restart nginx
aperte a tecla "enter"

DIGITE
sudo reboot now
aperte a tecla "enter"

FECHE O "TERMINAL" / "New SFTP window" / "BITVISE"

COPIE A "URL" DO FRONTEND E COLE NO GOOGLE CHROME E APERRTE A TECLA "ENTER"

DADOS PARA O PRIMEIRO LOGIN

admin@admin.com
123456

fim

NOSSO SUPORTE FUNCIONA DE SEGUNDA Á SABADO DE 15 A 19 HORAS.

------------------------------------------
VARIAVEIS QUE PODEM SER USADAS DENTRO DO PAINEL

{{ms}} - Bom dia, boa tarde, boa noite ou boa madrugada dependendo da hora do dia

{{name}} - Nome cadastrado no WhatsApp de quem entrou em contato

{{protocol}} - Geração de protocolo



---------------------------------------------------------------------------------------------------------------------------------------------------------
---------------------------------------------------------------------------------------------------------------------------------------------------------
---------------------------------------------------------------------------------------------------------------------------------------------------------
---------------------------------------------------------------------------------------------------------------------------------------------------------
---------------------------------------------------------------------------------------------------------------------------------------------------------


FAZENDO DOWNLOAD DO INSTALADOR & INICIANDO A PRIMEIRA INSTALAÇÃO (USAR SOMENTE PARA PRIMEIRA INSTALAÇÃO):

```bash
sudo apt install -y git && git clone https://github.com/cronoswebdigital/instaladorSaas.git install && sudo chmod -R 777 ./install && cd ./install && sudo ./install_primaria
```

ACESSANDO DIRETORIO DO INSTALADOR & INICIANDO INSTALAÇÕES ADICIONAIS (USAR ESTE COMANDO PARA SEGUNDA OU MAIS INSTALAÇÃO:
```bash
cd && cd ./install && sudo ./install_instancia
```

