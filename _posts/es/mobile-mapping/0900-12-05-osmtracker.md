---
layout: doc
title: OSMTracker
permalink: /es/mobile-mapping/osmtracker/
lang: es
category: mobile-mapping
---

OSMTracker
==============

> Esta guía puede ser descargada como  [OSMTracker_es.odt](/files/OSMTracker_es.odt) o [OSMTracker_es.pdf](/files/OSMTracker_es.pdf)  
> Revisado 2015-07-17
  
**Este artículo se refiere a OSMTracker para Android - existe un producto similar disponible para Windows Mobile.**  
OSMTracker permite crear una traza GPX de un viaje, con la colección de los 'puntos de ruta' a lo largo de la ruta. Grabaciones de voz, fotografías y otras notas también pueden ser registradas, y todas serán geolocalizadas.

Inicio rápido
-----------
![OSMTracker_1][]

1. Haz clic en la cruz para crear una nueva traza.  
2. La pantalla cambiará para mostrar los botones - espera hasta que ya no estén en gris, lo que indica que el GPS tiene la posición.  
3. Viaje por su ruta, pulsando los botones apropiados cuando se encuentres exactamente en la característica a ser mapeada. También puede crear grabaciones de voz, tomar fotografías y tomar notas utilizando los botones.  
4. Cuando haya terminado, pulse el icono del disquete para guardar la traza y los puntos de ruta.
5. Para convertir la traza en un archivo gpx, pulse y mantenga en la lista, luego seleccione la opción adecuada.
6. Transfiera la traza, fotos y grabaciones a su equipo y lea desde ellas para actualizar OSM.


Instala OSMTracker
-------------------------

Instala OSMTracker desde la [Tienda Google Play](https://play.google.com/store/apps/details?id=me.guillaumin.android.osmtracker).  
![OSMTracker Logo][]  
El [paquete de la aplicación más reciente](https://drive.google.com/folderview?id=0BxxhTXmYjyeSSjg1MFhJWnJLams#list) puede ser descargado fuera de la Tienda Google Play si fuese necesario.  


Configuración OSMTracker
------------------------

Inicie OSMTracker, y presione el icono del menú en su dispositivo Android, luego seleccione **Ajustes**.  

- **La duración de la grabación de voz** -  a su elección, pero 30 segundos es utilizada por el autor.  
- **Habilitar sonido** - recomendado marcar esta casilla - emite un pitido de advertencia cuando la grabación comienza y termina.  
- **Restablecer la autenticación**. Este botón estará en 'color gris'  hasta que tenga subido un archivo .gpx, y autorice a OSMTracker a subir trazas a su cuenta OpenStreetMap.  
- **Ajustes GPS** Qué métodos de su dispositivo Android utilizará para determinar la ubicación. Es recomendado establecer esto a **Alta precisión** y así el dispositivo utilizará GPS, Wi-Fi y las redes móviles para estimar la ubicación.  
- **Comprobar el GPS al iniciar** Al iniciar OSMTracker, si el GPS ha sido apagado, la aplicación le preguntará que lo active de nuevo.
- **Ignorar el reloj GPS** Si está marcado se usará el reloj interno de los dispositivos en lugar del tiempo provisto por la señal GPS.  
- **Intervalo de registro GPS** Escoger el periodo entre el registro de la posición - para la mejor precisión elegir 0 o 1, cada uno de los cuales resulta en un registro cada segundo.  
  >La frecuencia afecta el uso de la batería; sin embargo, cuando utiliza usted esta aplicación, es probable que su pantalla esté encendida la mayor parte del tiempo, el gps esté en función, y que usted pueda estar tomando fotografías y también grabando -todo esto resultará en un agotamiento severo de la batería y es recomendable para uso extendido que se utilice el dispositivo con mayor energía.  
- **Directorio de almacenamiento externo (SD)** Por defecto es /osmtracker  
  >Algunos dispositivos Android recientes no permiten guardar datos en una microSD o tarjeta SD. Aunque se indique como 'dispositivo externo' las trazas se guardarán en **/storage/emulated/0/osmtracker.**  
-  **Un directorio por traza** Se recomienda ya que esto resultará en que todas las grabaciones de voz, fotografías, notas de texto y la traza gpx se almacenen en el mismo directorio, cuyo nombre será la fecha y la hora de creación del archivo gpx.  
-  **Nombre del archivo para las trazas** Algunas opciones para que puedas elegir el nombre con que se guardarán las trazas.  
-  **Precisión en el archivo GPX** Recomendado - Esto resultará en que el nombre de los puntos de ruta incluyan una cifra con un posible rango de error en metros. Por ejemplo *Sendero (4.0m)*. Esta información puede ser extremadamente útil cuando se actualice OSM y se tenga que decidir si se desea mover un objeto existente para alinearlo con la nueva traza y sus puntos de ruta.  
-  **Usar aproximación HDOP** Esto se relaciona con algunos cálculos adicionales para mejorar la precisión en la posición (precision de dilución horizontal).  
-  **Exportar la dirección de la brújula** Define el si y el cómo se desean exportar los datos de la brújula al archivo GPX.  

-  **Fuente de fotos predeterminado** Generalmente tomarás fotografías con la cámara a través de esta app, pero puedes elegir si deseas usar fotografías que ya están en el teléfono.  
-  **Pantalla siempre encendida** Selecciona esto si estás constantemente presionando los botones, tomando fotografías o haciendo grabaciones de voz - Si no lo estás haciendo, deja la opción vacía, así tendrás que encender la pantalla cada vez; esto gastará menos batería.  
-  **Tema de la pantalla principal** Opciones para cambiar el contraste y el brillo en caso de que estés teniendo problemas para ver los botones.  
-  **Preajustes de los botones** Tu puedes diseñar e instalar tus propios botones y hacer que se muestren. Para una descripción completa de esta función, [Ver abajo](/es/mobile-mapping/osmtracker/#button-presets).   
-  **Mapa de fondo** Si esta característica está seleccionada, al mantener presionado sobre una traza, esta se mostrará y además la app descargará como fondo los datos de OpenStreetMap.  
  > Para descargar el mapa se requiere una conexión de datos. No necesitas usar esta función a menos que quieras.
-  **Proveedor de teselas de mapa** Si has seleccionado descargar un mapa como fondo, puedes seleccionar qué versión del mapa deseas usar como fondo.  
-  **Orientación**  ¿Deseas que la pantalla rote, o deseas usarla en modo paisaje o retrato?

Sobre la lista de trazas
--------------

![OSMTracker_2][]  
Una vez que hayas concluido tu reconocimiento inicial, después de haber presionado algunos botones, creado grabaciones de voz y tomado algunas fotografías, haz click en el icono del disco floppy  para finalizar tu traza. Ahora presiona y mantenga presionado sobre la traza para visualizar las opciones:  

-  **Reanudar la traza** ¡Muy útil cuando te das cuenta que te haz olvidado de trazar algo!  
-  **Mostrar** Esto mostrará la traza, posiblemente con un mapa de fondo dependiendo de tu conexión de datos y la opción que hayas seleccionado en **Mapa de fondo**.  
-  **Exportar como GPX** - Opción necesaria para que la traza y los puntos de ruta puedan ser utilizados en algún programa de edición.  
-  **Subir a OpenStreetMap** Utiliza esta opción para subir tu traza a OpenStreetMap - es necesario tener una cuenta en OpenStreetMap ([Aquí se explica como obtener una](/es/beginner/start-osm/)), y autorizar que esta app pueda subir las trazas a tu cuenta. Ver [Trazas GPS - Archivos GPX abajo](/es/mobile-mapping/osmtracker/#gps-traces--gpx-files) para más información sobre por qué esas trazas son tan importantes para OpenStreetMap.  
>**Precaución, aún no elimines tu traza.** Solo haz subido la traza básica sin los puntos de ruta, fotografías, etc. Conserva todo mientras esto se transfiere a una computadora para fines de edición.  

-  **Eliminar**. Se explica solo.  


Sobre los preajustes de los botones.
--------------
Si te encuentras mapeando por alguna razón en particular, y el botón de punto de ruta que requieres no se encuentra disponible, puedes crear tus propios botones antes de iniciar tu viaje, cargarlos en tu teléfono y seleccionarlos mientras mapeas, o cuando los necesites - se pueden cargar muchos y activarlos/desactivarlos sin detener la grabación de la traza. Como las etiquetas que generas se encuentran forma de notas personales, no se necesita que estas cumplan con las etiquetas utilizadas en OpenStreetMap, además de que no subirán. Por ejemplo, puedes elegir tener tus botones con etiquetas.  
1 familia,  
2 familias,  
3 familias,  
4 familias,  
casa principal,  
Dañado 20%,  
Dañado 40%,  
Dañado 60%,  
Dañado 80%,  
destruído,  
inadecuado para camión,  
necesario un 4x4,  
etc..  

Para una descripción completa sobre creación de botones, ver [OSMTracker wiki section](https://github.com/nguillaumin/osmtracker-android/wiki/Custom-buttons-layouts). Aquí un ejemplo: [sample download file.](/files/R_of_Way.xml)

![OSMTracker button presets][]


Tamaño de las grabaciones de voz, fotografías e imágenes de texto.  
-----------------------------------------------  

![OSMTracker recorded file sizes][]

Si la transferencia de archivos es un problema, ten en cuenta el tamaño de los archivos involucrados -  como se muestra en la imagen, las fotografías hacen uso intensivo de la memoria en comparación con los archivos gpx o con las grabaciones de voz de 10 segundos.


Trazas GPS - archivos gpx 
----------------------  

![OSMTracker JOSM][]  
Las trazas GPS en forma de archivos gpx están compuestas de diversos elementos, principalmente una 'traza' y diversos 'puntos de ruta'. La imagen de abajo muestra el contenido de un directorio creado en OSMTracker, el cual ha sido cargado en JOSM para su edición, junto con imágenes satelitales como apoyo. El icono cuadrado en el centro de la traza indica que hay una fotografía disponible que fue tomada en ese lugar - solo debes presionar en el cuadro para mostrar la fotografía. 

Si te encuentras en marcha y estás usando el GPS para obtener instrucciones, en algún punto notarás que 'recalculará la ruta'. Esto se debe normalmente a que la ubicación interna del GPS no corresponde a donde espera encontrar una vía o camino - existe un margen de error, pero es fácil que las vías o caminos se construyan en lugares ligeramente erróneos, o que el camino sea movido una vez que los datos del mapa se han creado.  
Los voluntarios que mapean en OpenStreetMap pueden descargar todas las trazas que han sido subidas en su área y utilizarlas para:  

  1.  Trazar caminos y rutas a través de áreas que no se pueden ver mediante imágenes de satélite debido a las nubes, árboles, sombras, edificios, etc.  
  2.  Ajustar las imágenes de satélite para alinearlas correctamente - puede haber variaciones enormes con algunas de las imágenes.

A pesar de que una sola traza gpx puede ser muy útil, puede que no sea particularmente precisa e incluso puede que se encuentre hasta 30 metros fuera de lugar. Cuando hay varias trazas, se puede ver más fácilmente la ruta correcta de la vía o camino - por ejemplo en la imagen de abajo se muestran las trazas gpx de un poblado en donde las principales vías se pueden ver debido al volumen de las trazas.  

![OSMTracker_gpx][] 




[OSMTracker Logo]: /images/mobile-mapping/osmtracker_logo.png
[OSMTracker_1]: /images/mobile-mapping/OSMTracker_1.png
[OSMTracker_2]: /images/mobile-mapping/OSMTracker_2.png
[OSMTracker button presets]: /images/mobile-mapping/OSMTracker_presets.png
[OSMTracker recorded file sizes]: /images/mobile-mapping/OSMTracker_files.png
[OSMTracker_gpx]: /images/mobile-mapping/OSMTracker_gpx.png
[OSMTracker JOSM]: /images/mobile-mapping/OSMTracker_JOSM.png
