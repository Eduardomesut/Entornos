

 ## ¿Cómo podemos crear un repositorio remoto? - Eduardo


Añadir un repositorio remoto a un repositorio local existente

 Para añadir un repositorio remoto a un repositorio local existente, debemos ejecutar el siguiente comando desde el directorio donde se encuentra el repositorio local:

    $ git remote add <nombre_remoto> <url_remoto>

 Por ejemplo, para añadir el repositorio remoto que creamos en el apartado 02 a nuestro repositorio local, el comando sería el siguiente:

    $ git remote add origin https://github.com/UC3Music-e/test-repository.git

 Si queremos usar el protocolo ssh para subir y bajar código, el comando sería el siguiente:

    $ git remote add origin git@github.com:UC3Music-e/test-repository.git

Ejemplo

    $ git remote add origin https://github.com/UC3Music-e/test-repository.git





Resultado

origin https://github.com/UC3Music-e/test-repository.git (fetch)
origin https://github.com/UC3Music-e/test-repository.git (push)

Verificación

    $ git remote -v

origin https://github.com/UC3Music-e/test-repository.git (fetch)
origin https://github.com/UC3Music-e/test-repository.git (push)

   
¿Qué es el README.md? - Eduardo

El archivo README.md es un archivo de texto plano que contiene información sobre un proyecto de software. Se encuentra en el directorio raíz de un repositorio de GitHub, y es el primer archivo que los usuarios ven cuando visitan el repositorio.

El archivo README.md suele incluir información sobre los siguientes temas:

   -Descripción del proyecto: Qué hace el proyecto y por qué es útil.
   -Instrucciones de instalación: Cómo instalar el proyecto y comenzar a usarlo.
   -Documentación: Cómo usar el proyecto y resolver problemas.
   -Licencia: Información sobre los derechos de autor y el uso del proyecto.
   -Contribuciones: Cómo contribuir al proyecto.

El archivo README.md es una herramienta esencial para cualquier proyecto de software. Ayuda a los usuarios a entender qué hace el proyecto y cómo usarlo. También proporciona información importante sobre la licencia y las contribuciones.

Un buen archivo README.md debe ser claro, conciso y fácil de leer. Debe proporcionar toda la información que los usuarios necesitan para comenzar a usar el proyecto.

![README](https://github.com/Eduardomesut/Entornos/assets/93294713/2197b506-b8c3-4ab4-8a8c-57b20f236ba5)



   ## ¿Qué es Markdown?
 
   Markdown nació como herramienta de conversión de texto plano a HTML, fue creada en 2004 por John Gruber, y se distribuye de manera gratuita bajo una licencia BSD. Se trata de un lenguaje de marcado basado en un formato de texto plano.
   Se puede considerar Markdown como un método de escritura, sencillo de escribir, y que en todo momento mantiene un diseño legible. Esto te permitirá añadir formatos como negritas, cursivas o enlaces, lo que hará de tu escritura algo más        simple y eficiente.
    
   ## ¿Qué son y qué utilidad tienen las licencias?

Una licencia es un documento legal que otorga a una persona o entidad el derecho a usar o distribuir una obra protegida por los derechos de autor. Las licencias pueden ser otorgadas por el autor de la obra, por el titular de los derechos      de autor, o por un tercero con autorización de estos.

Las licencias tienen una gran utilidad, ya que permiten a los autores y titulares de derechos de autor controlar cómo se utiliza su obra. Las licencias pueden utilizarse para:

- Permitir que otros usen la obra de forma gratuita o por una tarifa.
- Permitir que otros adapten o modifiquen la obra.
- Permitir que otros distribuyan la obra.
- Permitir que otros usen la obra con fines comerciales.
   
## ¿Qué es el fichero .gitignore?

El fichero gitignore es una herramienta muy común en Git que sirve para excluir ficheros y directorios de del control de versiones.Aunque en ocasiones suele fallar y se podrían seguir rastreando algunos archivos o que no los escluyan.Normalmente,estos archivos .gitignore se suelen colcar en el directorio raiz de un proyecto o puedes crearte un archivo gitignore global, en el cual toda la información que le entre,la ignorará en todos los repositorios Git.

##    Explicar las tres formas de integrar el repo remoto en un repo local.

Hay dos maneras principales de integrar un repositorio remoto en un repositorio local:

- Traer los cambios del repositorio remoto: Este método descarga los cambios del repositorio remoto al repositorio local, pero no los fusiona en la rama actual. Esto permite ver los cambios realizados en el repositorio remoto sin que afecten a tu trabajo local.

  Para traer los cambios del repositorio remoto, utiliza el comando git fetch:

      git fetch <nombre_remoto>

  Por ejemplo, para traer los cambios del repositorio remoto llamado "origin", ejecuta el siguiente comando:

      git fetch origin

  Este comando descargará los cambios del repositorio remoto en la rama "origin/master".

- Fusionar los cambios del repositorio remoto: Este método descarga los cambios del repositorio remoto y los fusiona en la rama actual. Esto permite combinar los cambios realizados en el repositorio remoto con tu trabajo local.

  Para fusionar los cambios del repositorio remoto, utiliza el comando git pull:

      git pull <nombre_remoto>

  Por ejemplo, para fusionar los cambios del repositorio remoto llamado "origin", ejecuta el siguiente comando:

      git pull origin

  Este comando descargará los cambios del repositorio remoto y los fusionará en la rama actual.

La elección del método a utilizar depende de tus necesidades. Si solo quieres ver los cambios realizados en el repositorio remoto, utiliza el método "traer". Si quieres combinar los cambios realizados en el repositorio remoto con tu trabajo local, utiliza el método "fusionar".

- También puedes utilizar el comando git merge para fusionar los cambios del repositorio remoto en una rama específica. Para ello, especifica el nombre de la rama que quieres fusionar con el comando merge. Por ejemplo, para fusionar los cambios del repositorio remoto en la rama "desarrollo", ejecuta el siguiente comando:

      git merge origin/desarrollo

  Este comando fusionará los cambios de la rama "origin/desarrollo" en la rama "desarrollo".

Si los cambios realizados en el repositorio remoto entran en conflicto con tu trabajo local, Git te lo notificará. En este caso, tendrás que resolver los conflictos manualmente antes de poder fusionar los cambios.

 ## ¿Cada cuanto hay que realizar un commit?

   Sabiendo que un commit es un captura instantánea de guardado de los cambios preparados en un momento del proyecto, podríamos decir que los commit se efectuan al realizar ciertos cambios en tu proyecto o al terminar ese proyecto aunque también es aconsejable realizarlo cuando tu sientas que es importante dejar un marcador que te sirva como registro.

   ![Captura desde 2024-01-16 18-57-48](https://github.com/Eduardomesut/Entornos/assets/155988531/a7c168ff-9612-47ee-8c70-5af56e08c719)

   ![Hacer commit en la rama dev](https://github.com/Eduardomesut/Entornos/assets/93294713/941772cf-21e0-4ca1-851d-3679b1a085a1)


   
   ## ¿Cómo podríamos trabajar varias personas en el mismo proyecto?

   1. Tenemos que crear una nueva organización desde cero en github.
   2. Ya con la organización creada tendríamos que ir a los ajustes de la organización.
   3. En la sección de acceso debemos ir a Colaboradores y hacer click en añadir personas.
   4. Insertamos el nombre de usuario de las personas a las que quieres invitar y hacer click en agregar personas al repositorio así dando por terminado el proceso.




 ## Parte 2

## Creación de ramas en Git

Las ramas en Git son una forma de aislar el trabajo en un proyecto. Esto permite trabajar en diferentes características o versiones del proyecto al mismo tiempo, sin interferir entre sí.

Para crear una nueva rama en Git, utilizamos el comando git branch: 

Por ejemplo, para crear una nueva rama llamada dev, ejecutaríamos el siguiente comando:

        git branch dev

Una vez que hemos creado una nueva rama, podemos cambiar a ella con el comando git checkout:

Por ejemplo, para cambiar a la rama dev, ejecutaríamos el siguiente comando:

        git checkout dev

Ahora, estaremos trabajando en la rama dev y cualquier cambio que realicemos se almacenará en esa rama.

![creacion rama](https://github.com/Eduardomesut/Entornos/assets/93294713/68e12f77-1c92-4efe-9a99-4b09052e3adc)


## Ramas para desarrollo

En general, se recomienda utilizar ramas separadas para el desarrollo de nuevas características o versiones de un proyecto. Esto ayuda a mantener el código limpio y ordenado, y facilita la revisión y el control de versiones.

Por ejemplo, si estamos trabajando en una nueva característica para nuestro proyecto, podemos crear una nueva rama llamada feature/nueva-caracteristica. Una vez que hayamos terminado de desarrollar la característica, podemos fusionarla en la rama main.

## Ramas para pruebas

También podemos utilizar ramas para pruebas. Esto nos permite probar nuevas características o cambios en nuestro proyecto sin afectar a la versión principal.

Por ejemplo, si queremos probar un nuevo cambio en nuestro proyecto, podemos crear una nueva rama llamada test/cambio-nuevo. Una vez que hayamos probado el cambio y estemos satisfechos con él, podemos fusionarlo en la rama main.

## Ramas para mantenimiento

Las ramas también se pueden utilizar para el mantenimiento de un proyecto. Por ejemplo, si necesitamos realizar cambios en una versión anterior de nuestro proyecto, podemos crear una nueva rama a partir de esa versión. Una vez que hayamos realizado los cambios, podemos fusionarlos en la rama main.

## Regla de las ramas

Una regla general que se recomienda seguir es la regla de las ramas. Esta regla establece que la rama main o master solo debe contener la versión acabada del producto. Todas las demás ramas deben utilizarse para el desarrollo, las pruebas o el mantenimiento.

Esta regla ayuda a mantener la versión principal del proyecto limpia y ordenada, y facilita la revisión y el control de versiones.

