# Instalar y Habilitar Sequelize y Sequelize-CLI
- para migraciones, modelos, seeders y conexion con la Base de Datos

```js
console.log("Holamundo")
```

## 1. Instalar Sequelize
```bash
npm i sequelize
```
## 2. Instalar Sequelize-cli
```bash
npm install --save-dev sequelize-cli
```
## 3. Configurar .sequelizerc

```js
const path = require('path');

module.exports = {
    'config': path.resolve('src/config', 'database.json'),
    'models-path': path.resolve('src', 'models'),
    'seeders-path': path.resolve('src', 'seeders'),
    'migrations-path': path.resolve('src', 'migrations')
};
```
## 4. Iniciar un nuevo proyecto con sequelize-cli
```bash
npx sequelize-cli init
```

------
## Descargar e Instalar GIT
```
http://git-scm.com/
```
- Luego Instalar
- Para Configurar agregar usuario y correo
```
git config --global user.name "FIRST_NAME" 
git config --global user.email "micorreo@mail.com"
```
- Crear una cuenta github, bitbucket o Gitlab

## Inicializar un nuevo repositorio Local
- para clonar un repositorio
```bash
git clone
```
- para crear un nuevo repositorio
```bash
git init
```
- para ignorar archivos y/o carpetas creamos un archivo (.gitignore) y registramos los archivos y carpetas que no queremos subir al repositorio
```
/node_modules
/dist
package-lock.json
.env
```
## Registrar el repositorio remoto (GITHUB, GITBUCKET o GITLAB)
- en este caso con GITHUB
```
git remote add origin https://github.com/fasossa/backend_renacer_node_angular.git
```
------
## Para agregar todos los archivos al index
```
git add .
```
## Para agregar o registrar los cambios agregamos un mensaje commit(head)
```
git commit -m "Configuracion base del proyecto node"
```