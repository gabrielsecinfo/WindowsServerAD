# WindowsServerAD
Instalando serviços do Active Directory utilizando Windows Server 2012 R2


Configuração do Windows Server 2012 R2 como um servidor Active Directory.

Após a criação da máquina virtual com Windows server 2012 R2 e subir o sistema estando ok para configurá-lo. Abri o gerenciador do servidor e fui até adicionar recursos (add roles and features)
 <img src="windowsr2/image.png"/>

Agora abrimos o menu de instalação para poder instalar  o AD (active directory):
 
  <img src="windowsr2/image1.png">

 Com isso iremos escolher o tipo de instalação na qual podemos fazer a base ou a com serviços de acesso remoto no qual tem requerimento de baixar recurso de (VDI) 
  <img src="windowsr2/image2.png">
Aqui temos a escolha do servidor se irá ser selecionado a parti de um Virtual HD ou pelo pool

  <img src="windowsr2/image3.png">

Agora iremos adicionar o serviço de domínios do AD (Podemos ativar outros serviços, porém só ativei o AD DOMAIN SERVICES):
 
  <img src="windowsr2/image4.png">


Logo após tem a aba de features no qual podemos escolher para ser instalado por exemplo o sistema de backup do Windows server, mas coloquei para pular direto a confirmação.

  <img src="windowsr2/image5.png">



 
Ao terminar a instalação podemos estar promovendo o servidor para o controlador de domínio


  <img src="windowsr2/image6.png">


E nisso irá aparecer algumas funções, mas como estamos começando do zero, a gente criará uma arvore e colocando o nome do domínio.


   <img src="windowsr2/image7.png">

 

Colocar senha para modulo de restore de serviços

   <img src="windowsr2/image8.png">


OBS: Não tem como colocar delegação de domínios por que o DNS não foi instalado

  <img src="windowsr2/image9.png">

 

Após dar next até em checagem de requisitos no qual irá analisar se ele tem o requisito para uso. Se tiver OK tudo, só instalar.
  <img src="windowsr2/image10.png">

 

Após a instalação do serviço iremos abrir o gerenciador do servidor>ferramentas> active directory usuários e computadores.

   <img src="windowsr2/image11.png">
