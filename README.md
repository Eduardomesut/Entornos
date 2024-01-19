 ## Parte 1

 ## ¿Cómo podemos crear un repositorio remoto? - Eduardo
 LINK:
https://david-estevez.gitbooks.io/the-git-the-bad-and-the-ugly/content/es/crear-un-repositorio-remoto.html

Añadir un repositorio remoto a un repositorio local existente

 Para añadir un repositorio remoto a un repositorio local existente, debemos ejecutar el siguiente comando desde el directorio donde se encuentra el repositorio local:

    $ git remote add <nombre_remoto> <url_remoto>

 Por ejemplo, para añadir el repositorio remoto que creamos en el apartado 02 a nuestro repositorio local, el comando sería el siguiente:

    $ git remote add origin https://github.com/UC3Music-e/test-repository.git

 Si queremos usar el protocolo ssh para subir y bajar código, el comando sería el siguiente:

    $ git remote add origin git@github.com:UC3Music-e/test-repository.git

Ejemplo

    $ git remote add origin https://github.com/UC3Music-e/test-repository.git

![Captura desde 2024-01-12 15-52-51](https://github.com/Eduardomesut/Entornos/assets/93294713/ac6633d4-1087-4fdf-8903-f9e0bbe47d32)


Resultado

origin https://github.com/UC3Music-e/test-repository.git (fetch)
origin https://github.com/UC3Music-e/test-repository.git (push)

Verificación

    $ git remote -v

origin https://github.com/UC3Music-e/test-repository.git (fetch)
origin https://github.com/UC3Music-e/test-repository.git (push)

   
¿Qué es el README.md? - Eduardo
![imagen](https://github.com/Eduardomesut/Entornos/assets/93294713/2c05c59a-a741-4f53-b919-0c28d0291861)



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

   
   ## ¿Cómo podríamos trabajar varias personas en el mismo proyecto?

   1. Tenemos que crear una nueva organización desde cero en github.
   2. Ya con la organización creada tendríamos que ir a los ajustes de la organización.
   3. En la sección de acceso debemos ir a Colaboradores y hacer click en añadir personas.
   4. Insertamos el nombre de usuario de las personas a las que quieres invitar y hacer click en agregar personas al repositorio así dando por terminado el proceso.
