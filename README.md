
Repositório para verificar testes automatizados de QA Quality Assurance

Guia para configuração da máquina para realizar automação Mobile com Appium + Robot


Instalando o Python 3 

Caso tenha o Python 2 instalado, desinstalar antes – caso seja Mac, não desinstalar o Python original de fábrica.

Baixar pelo site “python.org/downloads/”

No prompt de comando (ou CMDER) executar os comandos abaixo para checar se o phyton e o pip foram instalados:

python –version

pip –version 


Instalando o JDK 8

https://www.oracle.com/java/technologies/javase/javase-jdk8-downloads.html 

Executar o comando “java -version” para checar a versão do Java instalada


JAVA_HOME

Criar uma variável de ambiente 

Este Computador > botão direito > Propriedades > Configurações avançadas do sistema > Variáveis de Ambiente > Variáveis de Sistema > Novo 

Nome da variável: JAVA_HOME
Valor da variável: C:\Programs File\Java\jdk1.8 ***

Abrir a variável de sistema “path” > Editar > Novo

Adicionar %JAVA_HOME%\bin


Android Studio

https://developer.android.com/studio

ir em Configure > AVD Manager


ANDROID_HOME

Criar uma variável de ambiente 

Este Computador > botão direito > Propriedades > Configurações avançadas do sistema > Variáveis de Ambiente > Variáveis de Sistema > Novo 

Nome da variável: ANDROID_HOME
Valor da variável: C:\Users\**seu usuário***\App\Local\Android\Sdk

Abrir a variável de sistema “path” > Editar > Novo

Adicionar as linhas abaixo:

%ANDROID_HOME%\platform-tools
%ANDROID_HOME%\tools
%ANDROID_HOME%\tools\lib
%ANDROID_HOME%\tools\bin


Appium

Baixar o Appium http://appium.io/ 

Adicionar as capabilities abaixo:

  "platformName": "Android",
  "deviceName": "Emulator",
  "app": "/Users/****/ .apk",
  "udid": "emulator-5554"


Robot Framework

Executar o commando: pip install robotframework

obs: pode ser que tenha que utilizar “pip3”

