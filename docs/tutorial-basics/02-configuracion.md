---
sidebar_position: 2
---

# Configuración del Entorno de Desarrollo

## ¿Qué es Node.js?

Node.js es una plataforma que permite a los desarrolladores utilizar JavaScript para crear aplicaciones no solo en los navegadores web, sino también en el lado del servidor. Antes, JavaScript solo se podía usar en el navegador, pero con Node.js, podemos utilizarlo para hacer cosas como crear servidores web, manejar bases de datos y realizar tareas de programación en el servidor.

La principal ventaja de Node.js es que es rápido y eficiente, lo que significa que puede manejar muchas cosas al mismo tiempo sin que la aplicación se bloquee o se vuelva lenta. Esto es especialmente útil para aplicaciones que necesitan manejar muchas conexiones a la vez, como aplicaciones de chat en tiempo real o redes sociales.

Además, Node.js viene con una herramienta llamada NPM que facilita la instalación de paquetes de código adicionales para agregar más funcionalidades a nuestras aplicaciones sin tener que escribir todo desde cero.

Node.js es una forma poderosa y versátil de utilizar JavaScript para crear todo tipo de aplicaciones, desde sitios web hasta aplicaciones móviles y de escritorio, permitiéndonos aprovechar las ventajas de JavaScript tanto en el navegador como en el servidor.

## Instalación de Node.js

Para instalar **Node.js**, simplemente dirígete a su página oficial.

![Node.js](/img/node.png)

La página de descarga detectará automáticamente la versión de tu sistema operativo. Como puedes observar en la página de descarga, aparecen dos versiones. Te recomiendo encarecidamente que descargues la versión LTS (Versión estable). Después de la descarga, ejecuta el archivo descargado.

![Node.js](/img/node1.png)

El proceso de instalación es sumamente sencillo, solo pulsa **Next** en cada pantalla o la opción por defecto. Una vez instalado Node.js, ejecuta el siguiente comando desde tu terminal. Para ello, puedes pulsar las teclas "windows" + "r", escribir "cmd" y pulsar intro. Luego, escribe el siguiente comando en la terminal:

```bash
node -v
```

Si a continuación te aparece el número de versión de Node.js, la instalación se ha efectuado correctamente. Para comprobar la instalación de npm, teclea el siguiente comando:

```bash
npm -v
```

## Instalación y configuración de MongoDB

### Conceptos previos

#### ¿Qué es MongoDB Atlas?

MongoDB Atlas es un servicio de base de datos administrado y alojado en la nube que ofrece MongoDB, una base de datos NoSQL ampliamente utilizada. En esencia, MongoDB Atlas proporciona una forma conveniente y escalable de alojar y administrar bases de datos MongoDB sin la necesidad de configurar y mantener servidores físicos.

Algunas de las características y ventajas de MongoDB Atlas incluyen:

1. **Infraestructura en la nube**: MongoDB Atlas se ejecuta en diferentes proveedores de servicios en la nube, como Amazon Web Services (AWS), Google Cloud Platform (GCP) y Microsoft Azure. Esto permite a los usuarios elegir la plataforma que mejor se adapte a sus necesidades y ubicación geográfica.

2. **Configuración sencilla**: MongoDB Atlas ofrece una interfaz de usuario intuitiva para crear y configurar clústeres de bases de datos MongoDB con pocos pasos. Esto facilita la creación de entornos de desarrollo, pruebas y producción.

3. **Escalabilidad**: MongoDB Atlas permite escalar verticalmente (agregar más recursos a una instancia existente) y escalar horizontalmente (añadir más nodos o réplicas al clúster) para adaptarse a la carga de trabajo y necesidades cambiantes.

4. **Seguridad**: El servicio incluye características de seguridad avanzadas, como cortafuegos de red virtual, acceso basado en roles, encriptación de datos en reposo y en tránsito, para proteger los datos almacenados en la base de datos.

5. **Copia de seguridad y recuperación ante desastres**: MongoDB Atlas ofrece opciones de copia de seguridad automáticas y la posibilidad de crear puntos de restauración para garantizar la disponibilidad y recuperación de datos en caso de errores o desastres.

6. **Monitoreo y métricas**: Proporciona herramientas para supervisar el rendimiento de la base de datos y la utilización de recursos en tiempo real, lo que ayuda a detectar problemas y optimizar el rendimiento.

7. **Actualizaciones y mantenimiento**: MongoDB Atlas maneja automáticamente las actualizaciones de software y el mantenimiento del sistema, lo que permite a los desarrolladores centrarse en la creación de aplicaciones sin preocuparse por la administración de la base de datos.

MongoDB Atlas es una solución conveniente y potente para alojar y administrar bases de datos MongoDB en la nube, lo que brinda a los desarrolladores una plataforma robusta y flexible para crear aplicaciones escalables y de alto rendimiento.

#### ¿Qué es MongoDB Compass?

MongoDB Compass es una herramienta gráfica de interfaz de usuario (GUI) proporcionada por MongoDB para facilitar la visualización, análisis y manipulación de datos almacenados en bases de datos MongoDB. Esta herramienta está diseñada para ayudar a los desarrolladores y administradores de bases de datos a interactuar con sus clústeres de MongoDB de una manera más intuitiva y eficiente, sin necesidad de utilizar comandos de línea de comandos.

Algunas de las características y funciones principales de MongoDB Compass incluyen:

1. **Exploración de datos**: Permite explorar y navegar por las colecciones y documentos almacenados en la base de datos de forma gráfica y organizada, lo que facilita la visualización de la estructura y los datos almacenados.

2. **Búsqueda y consulta**: Ofrece una interfaz para realizar consultas y búsquedas en la base de datos utilizando un generador de consultas visuales o la sintaxis de consulta de MongoDB.

3. **Visualización de datos**: Proporciona representaciones visuales de los datos almacenados en forma de tablas, documentos JSON o vistas de árbol, lo que ayuda a comprender mejor los datos y su relación.

4. **Edición y actualización**: Permite editar y actualizar documentos de manera interactiva, lo que facilita la modificación de datos sin necesidad de escribir comandos manualmente.

5. **Índices y estadísticas**: Proporciona información sobre los índices existentes en la base de datos y estadísticas de rendimiento, lo que ayuda a optimizar las consultas y mejorar el rendimiento general.

6. **Visualización de la estructura**: Muestra detalles sobre los campos y tipos de datos utilizados en los documentos, lo que facilita el diseño y modelado de la base de datos.

7. **Geolocalización**: Incluye herramientas para trabajar con datos geoespaciales y permite realizar consultas basadas en ubicaciones.

8. **Migración de datos**: Facilita la importación y exportación de datos entre diferentes bases de datos y colecciones, lo que es útil para tareas de migración y copia de seguridad.

MongoDB Compass es una herramienta valiosa para aquellos que prefieren una interfaz gráfica para interactuar con MongoDB, ya que ofrece una forma más amigable de trabajar con la base de datos sin sacrificar la potencia y flexibilidad que MongoDB ofrece.

### Configuración de MongoDB Atlas

Existen dos formas de utilizar MongoDB en nuestras aplicaciones. Una sería hacer una instalación local y la otra sería configurar nuestra base de datos en la nube con **MongoDB Atlas**. Nosotros escogeremos esta última modalidad, ya que es bastante eficiente y además MongoDB cuenta con una versión gratuita que podemos utilizar para realizar nuestras pruebas. Para crear nuestra base de datos, debes dirigirte a la página oficial de **MongoDB**: https://www.mongodb.com/es/atlas/database

![MongoDB Atlas](/img/mongo.png)

Una vez situado en esta página, solicita la **prueba gratuita** y regístrate. Una vez que tu cuenta ha sido registrada, inicia sesión. Deberá aparecerte la siguiente pantalla o similar:

![MongoDB Atlas](/img/install_mongo1.png)

En esta pantalla, pulsa el botón verde que dice **Construir una base de datos**. Se te aparecerá la siguiente página.

![MongoDB Atlas](/img/install_mongo2.png)

Escoja la opción gratuita. También escoja el proveedor y en **región**, la región más cercana a su país. Deje el resto de opciones como están. Se le aparecerá la siguiente pantalla: 

![MongoDB Atlas](/img/install_mongo3.png)

Escoja la opción de **Username and Password** y escriba su usuario y contraseña. Es importante apuntarse estos datos, pues serán imprescindibles para poder establecer conexión con nuestra BB.DD.
En la opción de **Add entry your IP address acces list**, pulse la opción **Add Entry". Esta opción sirve para especificar desde que IP's es accesible nuestra base de datos. Escriba 0.0.0.0, esto le indica a MongoDB que se puede acceder a nuestra BB.DD, desde cualquier IP. Esta opción debería estar registrada en un BB.DD de producción, pero como aquí vamos a utilizar esta base de datos con fines educativos no importa. Con esto ya tendríamos configurada nuestra base de datos.

## Instalación y configuración de MongoDB Compass

![MongoDB Atlas](/img/compass1.png)

Pulsa el botón **Connect** y en la ventana que viene a continuación, pulsa la opción **Compass**.

![MongoDB Atlas](/img/mongo5.png)

Se te aparecerá la siguiente ventana:

![MongoDB Atlas](/img/mongo6.png)

En caso de no tener MongoDB Compass, selecciona la opción marcada en rojo. Se te aparecerá la siguiente pantalla:

![MongoDB Atlas](/img/mongo7.png)

Selecciona tu sistema operativo y copia la cadena de conexión que se te ofrece (la utilizaremos más adelante). Descarga **MongoDB Compass**. El proceso es totalmente automático. Por último presione el botón **Domwload**.

### Configuración de MongoDB Compass 

Después de la instalación de **MongoDB Compass** si no se le ha desplegado automáticamente la Aplicación, se le habrá creado un acceso directo en el escritorio, haga doble Click sobre el mismo. 
Se te aparecerá la siguiente pantalla:

![MongoDB Compass](/img/mongo_connect.png)

Ahora en el recuadro de **New Connectión** que copiamos anteriormente. Sustituya el texto **"password"** por su password real incluidos los signos "<" y ">". Pulse el botón **Connect**. Listo, ya tenemos configurado nuestro entorno de trabajo. 

