# Conexión a MongoDB Atlas con Node.js
Este archivo README proporcionará instrucciones detalladas sobre cómo ejecutar el código JavaScript proporcionado para conectarse a una base de datos MongoDB en MongoDB Atlas utilizando el controlador oficial de MongoDB para Node.js.

# Crear una cuenta en MongoDB Atlas
Si aún no tienes una cuenta en MongoDB Atlas, sigue estos pasos para crear una cuenta gratuita:

Visita el sitio web de MongoDB Atlas: https://www.mongodb.com/cloud/atlas.

Haz clic en el botón "Registrarse" o "Comenzar gratis" para crear una cuenta.

Completa el formulario de registro con tu información personal y sigue las instrucciones para crear tu cuenta.

# Crear un clúster en MongoDB Atlas
Un clúster en MongoDB Atlas es un conjunto de servidores que alojarán tu base de datos. Sigue los siguientes pasos para crear un clúster en MongoDB Atlas:

Inicia sesión en tu cuenta de MongoDB Atlas.

Haz clic en el botón "Build a Cluster" o "Crear clúster" para crear un nuevo clúster de MongoDB. Puedes elegir la opción gratuita (M0) para empezar.

Selecciona la nube y la región en la que deseas alojar tu base de datos.

Configura las opciones adicionales según tus preferencias.

Haz clic en el botón "Create Cluster" o "Crear clúster" para iniciar el proceso de creación. Esto puede llevar unos minutos.

# Configurar acceso a la base de datos
Para conectarte a tu clúster en MongoDB Atlas, debes configurar el acceso a la base de datos siguiendo estos pasos:

Haz clic en la pestaña "Database Access" o "Acceso a la base de datos" en el panel de navegación izquierdo.

Haz clic en el botón "Add New Database User" o "Agregar nuevo usuario de la base de datos" para crear un usuario que tenga acceso a la base de datos.

Completa el formulario para crear un nuevo usuario y asegúrate de anotar las credenciales (nombre de usuario y contraseña) que elijas, ya que las necesitarás para la conexión.

# Configurar la seguridad del clúster
Para permitir que tu aplicación se conecte al clúster, debes configurar la seguridad siguiendo estos pasos:

Haz clic en la pestaña "Network Access" o "Acceso a la red" en el panel de navegación izquierdo.

Haz clic en el botón "Add IP Address" o "Agregar dirección IP" para agregar tu dirección IP actual. Esto permitirá que tu aplicación se conecte al clúster desde tu máquina local.

# Obtener la URI de conexión
La URI de conexión es una cadena de conexión que utilizaremos en el código para establecer la conexión con tu base de datos en MongoDB Atlas. Sigue estos pasos para obtener la URI de conexión:

Haz clic en la pestaña "Clusters" o "Clústeres" en el panel de navegación izquierdo y luego en el botón "Connect" o "Conectar" junto a tu clúster.

En la pantalla de conexión, elige la opción "Connect your application" o "Conectar tu aplicación".

Selecciona el driver "Node.js" y copia la URI de conexión proporcionada. Debería tener un formato similar a este:

mongodb+srv://<username>:<password>@<cluster-name>.mongodb.net/<database>?retryWrites=true&w=majority
Asegúrate de reemplazar <username> y <password> con las credenciales del usuario que creaste en el paso anterior, <cluster-name> y <database> ya vendrán modificadas con el cluster y base de datos que estés conectando.

Ahora que has creado una cuenta en MongoDB Atlas, configurado un clúster y obtenido la URI de conexión, estás listo para ejecutar el código y establecer la conexión con tu base de datos en MongoDB Atlas.

# Descargar el código
Clona o descarga el código fuente desde el repositorio correspondiente. Puedes seguir estos pasos para clonar el repositorio utilizando Git:

Abre una terminal.

Navega hasta el directorio donde deseas clonar el repositorio.

Ejecuta el siguiente comando para clonar el repositorio:

git clone <URL_DEL_REPOSITORIO>
Reemplaza <URL_DEL_REPOSITORIO> con la URL del repositorio que deseas clonar. Por ejemplo: git clone https://github.com/tu-usuario/tu-repositorio.

Esto creará una copia local del repositorio en tu sistema.

# Instalar dependencias
Abre una terminal y navega hasta el directorio donde clonaste el repositorio. Ejecuta el siguiente comando para instalar las dependencias necesarias: npm install
Esto descargará e instalará el controlador oficial de MongoDB para Node.js y todas sus dependencias.

# Configurar la URI de conexión
Abre el archivo donde se encuentra el código (index.js o similar) y busca la siguiente línea:
const uri = "mongodb+srv://<username>:<password>@<cluster-name>.mongodb.net/<database>?retryWrites=true&w=majority";
Reemplaza la URI de conexión con la que obtuviste de MongoDB Atlas. Asegúrate de que la URI esté entre comillas y que tenga el formato correcto. Recuerda reemplazar <username>, <password>, <cluster-name> y <database> con los valores correctos.

# Ejecutar el código
Una vez que hayas configurado la URI de conexión, estás listo para ejecutar el código y establecer la conexión con tu base de datos en MongoDB Atlas.

Abre una terminal y navega hasta el directorio donde se encuentra el código. Ejecuta el siguiente comando para ejecutar el script:
node index.js
Si todo está configurado correctamente, verás un mensaje de confirmación que indica que te has conectado exitosamente a MongoDB Atlas.

You successfully connected to MongoDB!
¡Felicitaciones! Ahora estás conectado a tu base de datos MongoDB en MongoDB Atlas utilizando Node.js.