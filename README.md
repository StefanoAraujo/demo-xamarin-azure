# Demo: Aplicativo Xamarin com back-end no Microsoft Azure

Neste repositório você terá acesso ao código-fonte de um aplicativo em Xamarin Forms, pronto para integração com back-end desenvolvido com o recurso Easy Tables.
Para acompanhar o hands on do vídeo, você precisará ter instalado em sua máquina uma versão do Visual Studio e uma conta no Microsoft Azure.

* Faça download gratuito do [Visual Studio Community 2015](https://aka.ms/mobile_downloadvisual). Após a instalação, faça a [configuração dos emuladores de android](https://aka.ms/android-emulator).
* Crie sua [conta gratuita no Microsoft Azure.](https://aka.ms/android-emulator)

## Criando o App Service

Na tela inicial do portal do Microsoft Azure, você deverá clicar no botão de **new (representação pelo símbolo +)** e localizar a opção ``Web + Mobile``. Ao clicar no menu, você encontrará
uma lista com alguns dos principais serviços disponíveis neste recurso. Para criar o back-end, vamos utilizar o ``Mobile App``. Na aba seguinte, vamos definir o nome da nossa aplicação, resource group e também habilitar o Application Insights.

<img width="822" alt="captura de tela 2016-11-25 as 23 04 48" src="https://cloud.githubusercontent.com/assets/2198735/20637128/f177de36-b363-11e6-851b-6180beace845.png">

## Acessando o App Service

Com o deploy concluído, teremos acesso ao dashboard do nosso aplicativo, nele conseguimos visualizar as principais informações e recursos disponíveis. Teremos, também, um gráfico resumido do Application Insights e no momento em que iniciarmos a utilização do back-end, registrará informações como requests e performance.

<img width="864" alt="captura de tela 2016-11-25 as 23 05 00" src="https://cloud.githubusercontent.com/assets/2198735/20637129/f1b4c08a-b363-11e6-8f24-0346ed24b78c.png">

## Conexão de Dados

O próximo passo é a criação da nossa Easy Tables e para isso precisamos criar uma data connection e um servidor. No menu lateral do dashboard do App Service, procure por Easy Tables e na sequência, clique
na barra azul com a legenda  ``Need to configure Easy Tables/Easy APIs - Click here to continue``. Selecione o tipo de conexão de dados, que pode ser SQL Database ou Storage e clique na opção abaixo do seletor para realizar as configurações necessárias.
Na aba que irá surgir, clique em ``Create new database`` e define o nome do banco.

**#DICA:** No item Pricing Tier, busque pela opção de server gratuito. Ele oferece 32MB de espaço e já é suficiente para começar a desenvolver e testar sua app.  

<img width="961" alt="captura de tela 2016-11-25 as 23 05 09" src="https://cloud.githubusercontent.com/assets/2198735/20637130/f1d6d148-b363-11e6-9edd-ea4f247bad28.png">

### Definição de servidor

Para criar o servidor, clicamos em ``Create new server``, definimos o nome, usuário e senha de acesso e a localização. 

**#DICA:** Para economizar, defina para o seu servidor a mesma região do seu App Service.

<img width="628" alt="captura de tela 2016-11-25 as 23 05 15" src="https://cloud.githubusercontent.com/assets/2198735/20637131/f1d9da8c-b363-11e6-929c-c8bc39a84b30.png">

### Inicialização do Aplicativo

Depois de criar a conexão de dados e o servidor, em alguns instantes o Microsoft Azure fará o deploy do serviço e o Easy Tables já os identificará como ativos. Com isso, basta você
inicializar o App, clicando no botão ``Initialize App``. Feito isso, já iremos para última etapa dentro do Microsoft Azure, que é criar as nossas tabelas de dados.

<img width="678" alt="captura de tela 2016-11-25 as 23 05 25" src="https://cloud.githubusercontent.com/assets/2198735/20637132/f1dbd2ec-b363-11e6-844f-1aafa9b023c4.png">

