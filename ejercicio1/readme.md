Ubicarse en un directorio (en escritorio):

$ cd desktop

Crear directorio ejercicios:

$ mkdir ejercicios

Ver contenido del directorio:
$ ls
ejercicio1/

Configurar usuario y correo globalmente:

Configuración de usuario:

$ git config --global user.name "Fernando HernandezR"

Para confirmar que usuario está registrado:
$ git config user.name
Fernando HernandezR


Configuración de correo:

$ git config --global user.email "ferhr.educativo@gmail.com"

Para confirmar que correo está registrado:
$ git config user.email
ferhr.educativo@gmail.com

Vamos a ubicarnos en la carpeta ejercicios y vamos a inicializar el repositorio:
Fernando@FliaHdezBrand MINGW64 ~/desktop/ejercicios
$ git init
Initialized empty Git repository in C:/Users/Fernando/Desktop/ejercicios/.git/

Verificar el estado de nuestro repositorio:
$ git status
On branch master

No commits yet

Untracked files:
  (use "git add <file>..." to include in what will be committed)
        ejercicio1/

nothing added to commit but untracked files present (use "git add" to track)

Realizar el primer commit:

Pasar archivos del área de trabajo al aera de preparación:
$ git add ejercicio1

Verifiquemos el estado:
$ git status
On branch master

No commits yet

Changes to be committed:
  (use "git rm --cached <file>..." to unstage)
        new file:   ejercicio1/readme.md


Si quisiéramos deshacer la acción de enviar el archivo al área de preparación, lo podrías realizar con el siguiente comando:
$ git rm –cached ejercicio1

Ahora si realicemos el commit:

$ git commit -m "Version Inicial"
[master (root-commit) 0d62e22] Version Inicial
 1 file changed, 0 insertions(+), 0 deletions(-)
 create mode 100644 ejercicio1/readme.md

Modificamos el archivo readme.md
$ git add ejercicio1

$ git status
On branch master
Changes to be committed:
  (use "git restore --staged <file>..." to unstage)
        modified:   ejercicio1/readme.md

$ git commit -m "Agrega solucion Primer Ejercicio"
[master 6633aa1] Agrega solucion Primer Ejercicio
 1 file changed, 74 insertions(+)

Si está seguro de agregar todos los cambios al siguiente commit, puede hacerlo asì:
$ git add .

Para mostrar el historial de commits que he realizado:
$ git log

