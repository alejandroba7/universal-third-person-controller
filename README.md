# Universal Third Person Controller
Universal Third Person Controller es un Package que modifica y agrega mecánicas al Starter Assets - Third Person Character Controller | URP de Unity Technologies para que podamos iniciar el desarrollo de nuestro videojuego sin tener que preocuparnos tanto por la programación.





# Como Instalar
1. Crea un nuevo proyecto en Unity.
2. Busca en el Package Manager de Unity el paquete Input System y dale instalar.
3. Unity te pedira reiniciar para activar el New Input System, dale si y reinicia Unity, se abre de nuevo el proyecto que creaste.
4. Descarga nuestro Package de Universal Third Person Controller e importa el paquete (Import Package) en tu proyecto.
5. Inicia a crear el videojuego de tus sueños.





# Características:
El Package contiene Scripts, Sprites, Prefabs, Escenas y otros recursos de ejemplo para entender mejor su ejecución y aplicación.

## Escenas:
UI: Escena con un ejemplo de menú inicio basico, control de datos,  compartir datos entre escenas, traducción de textos, control de sonidos e idioma.

Collect Items: Escena con un minijuego de recolectar items, menu pause y guardado de datos.

## UI:
MenuController: Script para crear un menú principal básico para tu videojuego, nos ayuda a controlar botones y paneles del canvas. 

PauseController: Script parecido a MenuController para crear un menú de pausa básico, nos ayuda a controlar botones y paneles del canvas.

LanguageController: Script para controlar el cambio de idiomas en la UI.

LanguageChange: Agrega este script a TextMeshProUI y controla la traducción del texto en diferentes idiomas. Es un sistema para controlar traducción muy básica pero funcional.

AudioController: Script para controlar el AudioSource de la cámara y los efectos de sonido mediante botones y sliders.

VolumeController: Controla los sliders para subir o bajar el volumen de los AudioSource de la cámara y los efectos de sonido.





## Datos:

LoadData: Este script solo debe ser llamado una vez cuando se inicia el juego para cargar los datos guardados y si no existen crear el archivo para guardarlos. También verifica el lenguaje de sistema operativo en el que se está ejecutando el juego para ayudarnos a traducir textos con el LanguageController.

ShareData: Nos permite compartir datos entre escenas, muy útil para cuando deseamos que el jugador pase de una escena a otra conservando información de salud, cantidad de municiones, ítems y otros, sin tener que volver a cargar toda esa información desde la base de datos.

PlayerData: Script básico que podemos modificar para agregar datos que deseamos manipular y guardar de nuestro jugador.

SaveSystem: Script que nos permite guardar en binario los datos del script PlayerData.

LevelStatus: Script que controla el estado del nivel actual.





## Mecánicas para el jugador:

1. Correr On/Off: Botón tipo On/Off para activar la mecánica de correr.

2. Sensibilidad de rotación y movimiento de la cámara: Variable para modificar la sensibilidad de rotación y movimiento de la cámara.

3. Salto: El jugador puede realizar un salto para alcansar lugares u objetos a una altura distante.
   
4. Doble Salto: El jugador puede realizar un salto adicional en el aire para alcansar plataformas distantes, mecánica desactivable en el controlador.

   





## Mecánicas para objetos:

CollectItem: Script que permite a un objeto ser recolectado por el jugador y sumado a una variable.

Rotate: Permite a un objeto rotar sobre sus propios ejes.

RotateAround: Permite a un objeto rotar u orbitar alrededor de otro.

MobilePlatform: Permite a una plataforma moverse a una posición determinada y regresar a su posición inicial.



