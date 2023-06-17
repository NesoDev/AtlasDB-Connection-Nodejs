# Conexión a MongoDB Atlas con Node.js
Este archivo README proporcionará instrucciones detalladas sobre cómo ejecutar el código JavaScript proporcionado para conectarse a una base de datos MongoDB en MongoDB Atlas utilizando el controlador oficial de MongoDB para Node.js.

# Crear una cuenta en MongoDB Atlas
Si aún no tiene una cuenta en MongoDB Atlas, sigua estos pasos para crear una cuenta gratuita:

1. Visite el sitio web de MongoDB Atlas: https://www.mongodb.com/cloud/atlas.

2. Haga clic en el botón "Registrarse" o "Comenzar gratis" para crear una cuenta.

3. Completa el formulario de registro con tu información personal y sigue las instrucciones para crear tu cuenta.

# Crear un clúster en MongoDB Atlas
Un clúster en MongoDB Atlas es un conjunto de servidores que alojarán tu base de datos. Sigue los siguientes pasos para crear un clúster en MongoDB Atlas:

1. Inicie sesión en su cuenta de MongoDB Atlas.

2. Haga clic en el botón "Build a Cluster" o "Crear clúster" para crear un nuevo clúster de MongoDB. Puede elegir la opción gratuita (M0) para empezar.

3. Seleccione la nube y la región en la que deseé alojar tu base de datos.

4. Configure las opciones adicionales según sus preferencias.

5. Haga clic en el botón "Create Cluster" o "Crear clúster" para iniciar el proceso de creación. Esto puede llevar unos minutos.

# Configurar acceso a la base de datos
Para conectarte a tu clúster en MongoDB Atlas, debe configurar el acceso a la base de datos siguiendo estos pasos:

1. Haga clic en la pestaña "Database Access" o "Acceso a la base de datos" en el panel de navegación izquierdo.

2. Haga clic en el botón "Add New Database User" o "Agregar nuevo usuario de la base de datos" para crear un usuario que tenga acceso a la base de datos.

3. Complete el formulario para crear un nuevo usuario y asegúrate de anotar las credenciales (nombre de usuario y contraseña) que elija, ya que las necesitará para la conexión.

# Configurar la seguridad del clúster
Para permitir que su aplicación se conecte al clúster, debe configurar la seguridad siguiendo estos pasos:

1. Haga clic en la pestaña "Network Access" o "Acceso a la red" en el panel de navegación izquierdo.

2. Haga clic en el botón "Add IP Address" o "Agregar dirección IP" para agregar tu dirección IP actual. Esto permitirá que su aplicación se conecte al clúster desde tu máquina local.

# Obtener la URI de conexión
La URI de conexión es una cadena de conexión que utilizaremos en el código para establecer la conexión con su base de datos en MongoDB Atlas. Sigua estos pasos para obtener la URI de conexión:

1. Haga clic en la pestaña "Clusters" o "Clústeres" en el panel de navegación izquierdo y luego en el botón "Connect" o "Conectar" junto a tu clúster.

2. En la pantalla de conexión, seleccione la opción "Connect your application" o "Conectar tu aplicación".

3. Seleccione el driver "Node.js" y copia la URI de conexión proporcionada. Debería tener un formato similar a este:
'mongodb+srv://<username>:<password>@<cluster-name>.mongodb.net/<database>?retryWrites=true&w=majority'
Asegúrese de reemplazar <username> y <password> con las credenciales del usuario que creó en el paso anterior, no será necesario reemplazar <cluster-name> y <database> ya vendrán modificadas por defecto con el cluster y base de datos que estés conectando.

Ahora que has creado una cuenta en MongoDB Atlas, configurado un clúster y obtenido la URI de conexión, estás listo para ejecutar el código y establecer la conexión con tu base de datos en MongoDB Atlas.

# Descargar el código
Clone o descarge el código fuente desde el repositorio correspondiente. Puedes seguir estos pasos para clonar el repositorio utilizando Git:

1. Abra la terminal de Git.

2. Navege hasta el directorio donde deseas clonar el repositorio.

3. Ejecute el siguiente comando para clonar el repositorio: 'git clone <URL_DEL_REPOSITORIO>'
Reemplaza <URL_DEL_REPOSITORIO> con la URL del repositorio que deseas clonar. Por ejemplo: git clone https://github.com/tu-usuario/tu-repositorio.
Esto creará una copia local del repositorio en tu sistema.

# Instalar dependencias
Abra una terminal y navege hasta el directorio donde clonó el repositorio. Ejecute el siguiente comando para instalar las dependencias necesarias: 'npm install'
Esto descargará e instalará el controlador oficial de MongoDB para Node.js y todas sus dependencias.

# Configurar la URI de conexión
Abra el archivo 'app.js' en un su IDE de preferencia y busque la siguiente línea:
'const uri = "mongodb+srv://<username>:<password>@<cluster-name>.mongodb.net/<database>?retryWrites=true&w=majority";'
Reemplaze la URI de conexión con la que obtuvo de MongoDB Atlas. Asegúrese de que la URI esté entre comillas dobles y que tenga el formato correcto. Recuerde reemplazar <username>, <password> con los valores correctos.

# Ejecutar el código
Una vez que haya configurado la URI de conexión, está listo para ejecutar el código y establecer la conexión con su base de datos en MongoDB Atlas.

Abra una terminal y navege hasta el directorio donde se encuentra el código. Ejecute el siguiente comando para ejecutar el script: 'node index.js'
Si todo está configurado correctamente, verá un mensaje de confirmación que indica que se ha conectado exitosamente a MongoDB Atlas.

You successfully connected to MongoDB!

¡Felicitaciones! Ahora estás conectado a tu base de datos MongoDB en MongoDB Atlas utilizando Node.js.
