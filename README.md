# JSON - SERVER
## Pasos de instalación
Para la instalación es necesario tener instalado `NodeJS` en cualquier versión. Podemos intalar Json-Server utilizando el siguiente comando:
```bash
npm install -g json-server
```
El cual realiza una instalación global, en este caso para pruebas instalaremos en modo desarrollo por lo que el comando será:
```bash
npm install -D json-server
```

Una vez terminada la instalación es necesario configurar nuestro `package.json`, creando un script de ejecución indicando el nombre del archivo a ejecutar:
```bash
"scripts": {
    "server" : "json-server --watch nombre_archivo.json"
},
```
Finalmente podemos ejecutar nuestro archivo el cual funcionará como una Api falsa, con el siguiente comando:
```bash
npm run server
```
esto levantará nuestro servidor falso y podremos realizar consultas.
## Primeros pasos
Para comenzar a utilizar, es importante conocer que la estructura que esta en formato JSON son capos que se pueden considerar rutas de nuestro backend, es decir:
```bash
// http://localhost:3000/posts
{
  "posts": [
    { "id": 1, "title": "json-server", "author": "typicode" }
  ]
}
```
Para poder realizar consultas es necesario contar con un cliente, que nos ayude a realizar peticiones http como ser `postman`. O bien el mismo navegador (No recomendado).
