---
title: Uso del 7º Bahía 
description:
type: “Docs”
tip: No elimine el formato fijo de la barra superior, la descripción es la descripción del artículo, si no se completa, se tomará el primer párrafo como contenido de referencia.
---
# Instalar y quitar la 7ª Bahía
## Preparativos:
Asegúrese de que el ZimaCube esté apagado y desconectado.
Prepare el disco duro que se instalará.
## Pasos Específicos:
Paso 1: Retire el panel frontal del gabinete.
![](https://manage.icewhale.io/api/static/docs/1722418820491_image.png)
Paso 2: Retire la 6ª bahía.
![](https://manage.icewhale.io/api/static/docs/1722418858886_image.png)
Paso 3: Gire en sentido antihorario para desenroscar los tornillos que aseguran la séptima unidad.
![](https://manage.icewhale.io/api/static/docs/1722418913222_image.png)
Paso 4: Retire la 7ª bahía.
![](https://manage.icewhale.io/api/static/docs/1722418964759_image.png)
![](https://manage.icewhale.io/api/static/docs/1722418974044_image.png)
Paso 5: Instale libremente el SSD en la 7ª bahía.
![](https://manage.icewhale.io/api/static/docs/1722419028169_image.png)
Paso 6: Empuje la 7ª bahía a la posición correcta y apriete los tornillos en sentido horario.
![](https://manage.icewhale.io/api/static/docs/1722419069919_image.png)

# Cómo actualizar el firmware de iluminación del 7º ZimaCube
*Para evitar fallos de esp32 en actualizaciones OTA (Over-The-Air), se introduce aquí un método de actualización por cable.*
## Solución de 3 pasos
1. Conéctese a WiFi
Conéctese a WiFi con una computadora
Nombre: "ZimaCube"
Contraseña: "homecloud"
2. Ingrese la URL
Ingrese en el navegador: 172.16.1.1
3. Suba el firmware
[https://drive.google.com/file/d/1h8LKvZ47gdMmpJzu6CFK3awjGFX5ayRE/view?usp=drive_link](https://drive.google.com/file/d/1h8LKvZ47gdMmpJzu6CFK3awjGFX5ayRE/view?usp=drive_link)

## Plan de respaldo

**Preparación antes de actualizar**
- Computadora
- Cable de datos tipo C
- Disco 7
- Descargue y descomprima el paquete comprimido
[https://drive.google.com/file/d/15nPalLy-2ieNQ84dT1gchBzLqtEfM--8/view?usp=drive_link](https://drive.google.com/file/d/15nPalLy-2ieNQ84dT1gchBzLqtEfM--8/view?usp=drive_link)

**Comenzar la actualización**
3.1 Use el cable de datos tipo C para conectar la computadora al puerto tipo C en el chip del séptimo disco.
3.2 Abra el enlace [espressif.github.io](espressif.github.io) en la computadora.
3.3 Haga clic en 'Conectar'
![](https://manage.icewhale.io/api/static/docs/1730360675989_image.png)

3.4 Seleccione el puerto serie para la conexión.
![](https://manage.icewhale.io/api/static/docs/1730360689217_image.png)

3.5 Haga clic en 'DIY'
![](https://manage.icewhale.io/api/static/docs/1730360715808_image.png)

3.6 Haga clic en 'Agregar Archivo' dos veces.
![](https://manage.icewhale.io/api/static/docs/1730360989529_image.png)

3.7 Cambie la dirección de grabado y seleccione el archivo.
*La dirección de grabado específica se muestra en la figura, seleccione los tres archivos después de la descompresión en orden.*
![](https://manage.icewhale.io/api/static/docs/1730360997291_image.png)

3.8 Haga clic en 'Programar' para iniciar la grabación.
![](https://manage.icewhale.io/api/static/docs/1730361017895_image.png)

3.9 La grabación está completa, presione el botón de reinicio RST, y el firmware se actualizó con éxito.