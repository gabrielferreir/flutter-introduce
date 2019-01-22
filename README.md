## O quê é Flutter?

Flutter é um SDK da Google para desenvolvimento mobile multiplataforma(Android, IOS) apartir de uma
unica base de código, ele foi apresentado em 2015 em um evento da linguagem Dart e tinha 
como objetivo renderizar de forma consistente a 120 fps. O lançamento inicial aconteceu em maio de 2017
e o lançamento da versão estavel(1.0.0) aconteceu no dia 4 de dezembro de 2018.

## Por que Flutter?
	* Produtividade (Base unica de codigo, Hot reload, Widgets prontos)
	* Crie experiencias de usuarios fodas e altamente personalizadas
    * Fluidez
    
![Galery](https://github.com/gabrielferreir/flutter-introduce/blob/master/images/galery-animation.gif)
![Galery](https://github.com/gabrielferreir/flutter-introduce/blob/master/images/galery-posse.gif)

## Flutter vs WebViews(Ionic/Cordova)

![WebViews](https://github.com/gabrielferreir/flutter-introduce/blob/master/images/webview.png)

As WebViews renderizam paginas web e como o Javascript não se comunica diretamente com o 
codigo nativo eles passam pela(Bridge) que // REVER ira se comunicar com o dominio nativo quando
for necessario se comunicar com serviços nativos.

## Ponte(Bridge)
![Bridge](https://github.com/gabrielferreir/flutter-introduce/blob/master/images/bridge.png)

A Ponte recebe seu codigo Javascript e realiza a mudança de contexto chamando os serviços 
nativos.

## Flutter vs React Native?

![reactive-views](https://github.com/gabrielferreir/flutter-introduce/blob/master/images/reactive-views.png)

Com o React-native não é diferente, ele não se comunica diretamente com o dominio nativo.
Mesmo que a maior parte do codigo do app seja escrito em Javascript a interface do usuario
é 100% nativa.
O react native trabalha em dois dominos diferentes o dominio nativo e o dominio do JS.
E ambos os dominios são extremamente rapidos. O problema acontece quando esse lados precisam se
comunicar, em casos em que são realizadas animações/transicoes esse reinos podem se comunicar ate 60 vezes
por segundos o que dificulta que o app rode a 60 fps e deixe seu app com uma fluidez legal.

## Flutter

![Flutter](https://github.com/gabrielferreir/flutter-introduce/raw/master/images/flutter.png)


O Flutter utiliza uma abordagem diferente, ele abandona a Brigde e utiliza uma linguagem 
complilada chamada Dart que complila em AOT (ahead of time) codigo nativo para multiplas 
plataformas.

## Fluter não utiliza os widgets OEM

![Evolution](https://github.com/gabrielferreir/flutter-introduce/raw/master/images/evolution.png)

Os widgets OEM são os widgets nativos de cada interface.
Porem isso não significa que você tera que criar seus Widgets do zero, Os Widgets de
ambas as plataformas estarão disponiveis para uso somente na versão mais recente do Material Designer.

##### Isso significa que seus usuario mais atentos podem ter surpresas...

![OEM](https://github.com/gabrielferreir/flutter-introduce/raw/master/images/oem.png)

#### Como o Flutter renderiza seus Widgets?

Comparado a outros frameworks o Flutter funciona de maneira totalmente diferente dos frameworks tradicionais
para criação de aplicativos, ele funciona de maneira semelhante a de um mecanismo de jogo.

O Flutter utiliza um mecanismo chamado Skia que recebe seus Widgets e envia as informações diretamente para o
canvas da plataforma e a plataforma retorna os eventos conforme necessario.

![Skia](https://github.com/gabrielferreir/flutter-introduce/raw/master/images/skia.png)

## Biografia

- <https://flutter.io/docs/resources/technical-overview>
- <https://hackernoon.com/whats-revolutionary-about-flutter-946915b09514>
- <https://medium.com/47billion/flutter-how-does-it-works-6e4c73842e67>
- <https://medium.com/the-andela-way/why-you-should-give-flutter-some-of-your-attention-22dd7e5cae42>
- <https://hackernoon.com/flutter-5-reasons-why-you-may-love-it-55021fdbf1aa>
- <https://medium.com/@talkol/performance-limitations-of-react-native-and-how-to-overcome-them-947630d7f440>
- <https://hackernoon.com/why-flutter-uses-dart-dd635a054ebf>
- <https://medium.com/flutter-io/why-flutter-doesnt-use-oem-widgets-94746e812510>
- <https://medium.com/flutter-community/flutter-platformview-how-to-create-flutter-widgets-from-native-views-366e378115b6>
- <https://buildflutter.com/how-flutter-works/>