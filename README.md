
  <h1>Meu Ambiente - Dockertoolbox - Selenium Grid </h1>
  
  <div id="PreparacaoAmbiente" class="tabcontent">
     <p><h3>1. Preparação do ambiente</h3></p>
     <h4>1.1 Fazer instalação</h4>
     <p><code>DockerToolbox (19.03.1 versão utilizada);</code></p>
     <p><code>Virtualbox (5.2.44 versão utilizada).</code></p>
      <h4>1.2 Docker compose</h4>
      <p> Baixar o <b>docker-composer.yml</b>, esse arquivo contem a imagem do <b>Selenium Grid</b> e os nós <b>Chrome</b> e <b>FireFox</b></p>
  </div>
  <div id="Setup" class="tabcontent">
     <p><h3>2. Setup Docker Toolbox </h3></p>
      <h4>2.1 Fazer a instalação do Docker Toolbox:</h4>
  </div>
  
  ![setup-01](https://user-images.githubusercontent.com/12755484/118699980-8238fa80-b7e8-11eb-9baf-52d0687ba949.png)

  <p>:x: Desmarque a opção VirtualBox </p>
  
 ![setup-02](https://user-images.githubusercontent.com/12755484/118700458-130fd600-b7e9-11eb-9c1e-99014a61379d.png)

   <h4>2.2 Fazer a instalação do Virtualbox:</h4>
 
 ![setup-3](https://user-images.githubusercontent.com/12755484/118701404-0fc91a00-b7ea-11eb-9c72-01255b832d2e.png)

   <h4>2.3 Após a finalização da instalação, abrir o Quickstart Terminal: </h4>
   
  ![setup-4](https://user-images.githubusercontent.com/12755484/118702318-2b80f000-b7eb-11eb-923f-2ed7c9e55b28.png)

   <p>Ao abrir o Quickstart, iniciará a criação da máquina virtual com o Docker configurado: </p>
  
  ![setup-5](https://user-images.githubusercontent.com/12755484/118703195-35572300-b7ec-11eb-8494-b5300c62c38e.png)
  
  ![setup-6](https://user-images.githubusercontent.com/12755484/118703339-5fa8e080-b7ec-11eb-84d0-d17c3d0c7202.png)

   <div id="ConfiguracaoRedeVirtualbox" class="tabcontent">
     <p><h3>3. Configuração de rede virtualbox </h3></p>
     <p>virtualbox deve ser configurada com as regras de redirecionamento de portas, acessar o menu na Virtualbox <b>configurações/Rede</b>:</p>
     <p>1. Informar o endereço <b>IP do Hospedeiro</b>: 172.0.0.1:4444</p>
     <p>2. Informar o endereço <b>IP do Convidado</b>: 192.168.99.100:4444</p>
  </div>
    <div id="ConfiguracaoRedeVirtualbox" class="tabcontent">
     <p><h3>4. Executar comando Docker-compose </h3></p>
     <p>Abra o terminal Quickstart e acesse o diretório onde está o <b>docker-composer.yml</b>:</p>
  </div>
  
  ![setup-7](https://user-images.githubusercontent.com/12755484/118706982-5cafef00-b7f0-11eb-8758-ff470a4e5115.png)

   <p>Execute o comando: <code>docker-compose up -d</code></p>
   
  ![setup-8](https://user-images.githubusercontent.com/12755484/118706661-06db4700-b7f0-11eb-8b2e-f5fc89dff562.png)
  
   <p>O docker iniciará o pull das imagens e criação dos containers: </p>
   
   ![setup-9](https://user-images.githubusercontent.com/12755484/118707447-ed86ca80-b7f0-11eb-8835-418db4618496.png)

   ![setup-10](https://user-images.githubusercontent.com/12755484/118707947-8289c380-b7f1-11eb-9ad6-fe952484d416.png)
   
   <p> Ao finalizar, execute o comando <code>docker ps -a para visualizar os containers executando:</code></p>
   
   ![setup-11](https://user-images.githubusercontent.com/12755484/118708317-f4faa380-b7f1-11eb-9a75-60af7dffb385.png)

   


