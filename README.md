#Creando un paquete

## Creando un nuevo proyecto repo vacio

### Paso 1 - Inicializa Git en la carpeta actual
git init		(Mensaje: Initialized empty Git repository in C:/laragongo/usr/go/src/github.com/emanchego/helloworld/.git/)

### Paso 2 - Muestra el estado actual de los archivos 
git status		(Mensaje: Lista de archivos y estado)

### Paso 3 - Agrega nuevos archivos a versionar
git add .		(Mensaje: Nada)

### Paso 4 - Configurando usuario (Solo es necesario la primera vez)
git config --global user.email "xxxxx@gmail.com"
git config --global user.name "xxxxxx"

### Paso 5 - Agregar mensaje 
Git commit -m "Commit inicial" (Mensaje: 1 file changed, 10 insertions(+))

### Paso 6 - Accedemos a github y creamos repo vacio
 
### Paso 7 - Agregamos direccion del repo
git remote add origin git@github.com:fire-fox/goHello.git

### Paso 8 - Revisar llaves
ssh -vT git@github.com
ls -al ~/.ssh

#### Paso 8.1 - Crear llaves si no hay
ssh-keygen -t rsa -b 4096 -C "erikmanchego@gmail.com"

#### Paso 8.2 - Añadir llaves a Github.com si no esta
Copiar contenido de id_rsa.pub
Pegar el contenido en github.com->settings->ssh keys

### Paso 9 - Subiendo los archivos
git push -u origin master

### Paso 10 - Configuracion terminada
Para hacer cambios seguir pasos 2, 3 , 5 y 9
