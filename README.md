Parte 1

¿Cómo podemos crear un repositorio remoto? - Eduardo
 LINK:
https://david-estevez.gitbooks.io/the-git-the-bad-and-the-ugly/content/es/crear-un-repositorio-remoto.html

Añadir un repositorio remoto a un repositorio local existente

 Para añadir un repositorio remoto a un repositorio local existente, debemos ejecutar el siguiente comando desde el directorio donde se encuentra el repositorio local:

*$ git remote add <nombre_remoto> <url_remoto>*

 Por ejemplo, para añadir el repositorio remoto que creamos en el apartado 02 a nuestro repositorio local, el comando sería el siguiente:

*$ git remote add origin https://github.com/UC3Music-e/test-repository.git*

 Si queremos usar el protocolo ssh para subir y bajar código, el comando sería el siguiente:

 *$ git remote add origin git@github.com:UC3Music-e/test-repository.git*

Ejemplo

*$ git remote add origin https://github.com/UC3Music-e/test-repository.git*

![Captura desde 2024-01-12 15-52-51](https://github.com/Eduardomesut/Entornos/assets/93294713/ac6633d4-1087-4fdf-8903-f9e0bbe47d32)


Resultado

origin https://github.com/UC3Music-e/test-repository.git (fetch)
origin https://github.com/UC3Music-e/test-repository.git (push)

Verificación

*$ git remote -v*

origin https://github.com/UC3Music-e/test-repository.git (fetch)
origin https://github.com/UC3Music-e/test-repository.git (push)

   
¿Qué es el README.md? - Eduardo
![imagen](https://github.com/Eduardomesut/Entornos/assets/93294713/2c05c59a-a741-4f53-b919-0c28d0291861)



    ¿Qué es Markdown?
    ¿Qué son y qué utilidad tienen las licencias?
    ¿Qué es el fichero .gitignore?
    Explicar las tres formas de integrar el repo remoto en un repo local.
    ¿Cómo realizar un commit? 
    ¿Cada cuanto hay que realizar un commit? - Garrido
    ¿Cómo podríamos trabajar varias personas en el mismo proyecto? - Garrido




hola esto es un ejemplo
segundo commit