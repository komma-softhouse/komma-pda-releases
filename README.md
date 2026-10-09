# Komma PDA

La PDA de almacén y tienda de **Komma ERP**. Hace inventarios, prepara envíos a otras tiendas, comprueba lo que llega de otras tiendas y de proveedores, consulta stock e IMEI y ficha a los empleados. Una lectura por unidad, con el láser de la PDA o con la cámara, y sigue trabajando aunque se caiga la red.

## Descargar

| Sistema | Descarga |
| --- | --- |
| **Android 13 o posterior** | [Última versión](https://github.com/komma-softhouse/komma-pda-releases/releases/latest) — el archivo `.apk` |

Todas las versiones publicadas están en [Releases](https://github.com/komma-softhouse/komma-pda-releases/releases). Cada versión trae también su archivo `.sha256` para comprobar que el `.apk` no se ha alterado. Lo más cómodo es descargarla desde el propio ERP, en **Sistema → Apps de tienda**, que siempre enlaza la última versión.

<p>
  <img src="assets/02-home.jpeg" width="200" alt="Inicio">
  <img src="assets/04-count-reading.jpeg" width="200" alt="Recuento">
  <img src="assets/09-reception-check.jpeg" width="200" alt="Recepción de un envío">
</p>

## Qué hace

- **Recuento de inventarios.** La oficina abre el inventario en el ERP y la PDA lee cada unidad: por IMEI o número de serie si lo tiene, por código de barras si no. Cada lectura sale en verde, ámbar (esperando al ERP) o rojo con el motivo.
- **Envíos a otras tiendas.** Empieza un envío o abre uno que preparó la oficina, lee lo que va en la caja y envíalo. Sin red se guarda todo y sale en orden cuando vuelve la conexión.
- **Recepción de envíos.** Al llegar un envío de otra tienda se comprueba unidad a unidad; lo que falta o sobra le llega a la oficina anotado en el envío.
- **Recepción de albaranes de proveedor.** Se comprueban las cajas contra el albarán y, si la oficina no tecleó los IMEI, se leen al llegar, unidad a unidad.
- **Consultas.** Stock de un artículo en esta tienda por color, stock en las demás tiendas y el recorrido completo de un IMEI.
- **Fichaje.** Cada empleado ficha con su código personal, aunque no haya red.
- **Sin red.** Todo lo que se lee queda guardado en la PDA y llega al ERP en orden; las barras de arriba dicen si el ERP responde y cuántas cosas esperan.
- **Se actualiza sola.** Desde **Ajustes → Actualizaciones**, sin pasar por Google Play.

## Instalar

1. En la PDA, abre la [última versión](https://github.com/komma-softhouse/komma-pda-releases/releases/latest) y descarga el archivo `.apk`.
2. Ábrelo. Si Android pide permiso para instalar apps de esta fuente, actívalo para el navegador y vuelve.
3. Pulsa **Instalar**. Komma PDA queda en el cajón de aplicaciones.

## Ponerla en marcha

1. **En el ERP**, entra en **Cajas e impresión → Terminales → Emparejar una PDA** y elige la tienda o el almacén. Aparece un código y su QR, válidos 15 minutos y para un solo uso.
2. **En la PDA**, pulsa **Leer el QR del ERP** y apunta al QR (o escribe la dirección del ERP y el código), pon un nombre a esta PDA y pulsa **Emparejar**. Se descargan los artículos, las tiendas, los empleados, el stock de su tienda y el trabajo pendiente.
3. **Entra con tu código personal.** Solo pueden entrar los empleados que en el ERP tienen acceso a PDA.
4. **Lector láser:** si la PDA tiene lector integrado, déjalo en modo teclado con Intro al final. La cámara funciona en cualquier móvil.

<p>
  <img src="assets/01-sign-in.jpeg" width="200" alt="Entrada con código">
  <img src="assets/06-shipment.jpeg" width="200" alt="Un envío">
  <img src="assets/10-lookup.jpeg" width="200" alt="Consulta">
</p>

## Requisitos

- Android 13 o posterior.
- Cámara trasera, o lector láser integrado en modo teclado.
- Wifi o datos para hablar con el ERP de la empresa. El recuento, los envíos y el fichaje aguantan sin red; abrir un envío o un albarán que llega necesita el ERP una vez.

## Actualizaciones

En **Ajustes → Actualizaciones** pulsa **Buscar actualizaciones**. Si hay una versión nueva, **Descargar e instalar** la baja, comprueba que ha llegado entera y abre el instalador de Android. La primera vez Android pide permitir instalar desde Komma PDA. La PDA conserva su emparejamiento y todo lo que tenga pendiente de enviar.

## Si algo falla

Cuando la PDA encuentra un error inesperado muestra un código de incidencia y un botón para informar del error. El informe llega a Komma con el código, la versión y la pantalla, sin datos de stock ni de empleados. Si llamas a soporte, ten el código a mano.

## Soporte

Komma SoftHouse · [kommasofthouse.com](https://kommasofthouse.com) · info@kommasofthouse.com
