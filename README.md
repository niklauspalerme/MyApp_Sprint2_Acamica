
## 1) Antes de correr la app/api necesitas:

 - Descargar el codigo de la branch **"main"**
 - Haber descargado **XAMPP** en tu computador y correrlo/inicicializarlo
![XAMPP](https://github.com/niklauspalerme/imagenes/blob/main/MyApp_Sprint2_Acamica/imagen%207.JPG)

  - Descargar **redis** en el puerto default **6379**

 - Haber descargado **POSTMAN** en tu computador y correrlo/inicicializarlo:
    - Importar la colección que se encuentra el a carpeta **Postman Collection**
![Postman collection](https://github.com/niklauspalerme/imagenes/blob/main/MyApp_Sprint2_Acamica/imagen%209.JPG)

 - Luego debes crear un archivo llamado **.env** afuera de la carpeta **src** como se muestras en la imagen

![Postman collection](https://github.com/niklauspalerme/imagenes/blob/main/MyApp_Sprint2_Acamica/Imagen%20%231.JPG)

- Una vez creado el archibo **env** debe copiar la información que esta en el archivo **sample** a **.env** y estará lista la aplicacion para correr localmente 

![App Screenshot](https://github.com/niklauspalerme/imagenes/blob/main/MyApp_Sprint2_Acamica/imagen%208.JPG)



## 2) Comandos para correr la app/api Local 

- Instalar el node_modules de la app/api en la carpeta principal (afuera de src)

 ```bash
  npm install
```

- Correr la app/api en la carpeta principal (afuera de src)

 ```bash
  npm run dev 
```

- **NOTA: La creación y las cargas de las tablas se hace de manera automatica una vez que se corre el comando "npm run dev" y si se tiene activo el XAMPP**

![Carga de la tablas](https://github.com/niklauspalerme/imagenes/blob/main/MyApp_Sprint2_Acamica/imagen%2010.JPG)

- Correr el test la app/api en la carpeta principal (afuera de src)

```bash
  npm run test
```


## 3) Postman Collection

- Se sugiere importar la coleción de Postman
- La colección de Postman va estar dividido por los diferentes endpoints

![postman division](https://github.com/niklauspalerme/imagenes/blob/main/MyApp_Sprint2_Acamica/imagen%202.JPG)

- La gran mayoria de los endpoints van a necesitar un token de **autenticación** en los headers para su uso:

![postman division](https://github.com/niklauspalerme/imagenes/blob/main/MyApp_Sprint2_Acamica/imagen%203.JPG)

- Se sugiere leer **la documentación de Swagger** para poder tener una idea de como usar cada unos de los endpoints

```bash
  http://localhost:8080/api-docs/
```

![documentación swagger](https://github.com/niklauspalerme/imagenes/blob/main/MyApp_Sprint2_Acamica/inmagen%204.JPG)

- En postman en la carpeta **User** va ver 2 pestañas para login. Una que va tener las credenciales del usuario admins, que les va servir para poder acceder a ciertos endpoints que estan restringidos

![login admins](https://github.com/niklauspalerme/imagenes/blob/main/MyApp_Sprint2_Acamica/imagen%205.JPG)

- Y la otra pestaña donde despuues de haber creado su usuario deberá colocar aqui los datos de login para poder tener su token de autenticación

![login usuario normal](https://github.com/niklauspalerme/imagenes/blob/main/MyApp_Sprint2_Acamica/imagen%206.JPG)

- Importante a tener en cuenta los token de autenticación van a tener un **Time Out** de 1 hr
