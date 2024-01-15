Parte 1

¿Cómo podemos crear un repositorio remoto? - Eduardo
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
    ¿Cómo realizar un commit? 
    ¿Cada cuanto hay que realizar un commit? - Garrido
    ¿Cómo podríamos trabajar varias personas en el mismo proyecto? - Garrido

