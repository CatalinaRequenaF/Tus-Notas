# Este es mi proyecto para apuntar notas:

![imagen](https://user-images.githubusercontent.com/91744454/220838404-387e77d1-f109-4fe5-b3d5-e1b305af3908.png)

![imagen](https://user-images.githubusercontent.com/91744454/220838863-82f29bc5-08c2-4fb4-9730-0382a145ceed.png)  

He escogido un diseño simpático y minimalista para que cualquier persona pueda usarlo sin problemas. He usado un color principal (verde) y variaciones, un color secundario (marrón grisáceo) y variaciones (gris) y para finalizar un color de resalte, el "rojo".
![imagen](https://user-images.githubusercontent.com/91744454/220844556-7aafa4fd-b75d-4646-ab60-999761af48d8.png)

![imagen](https://user-images.githubusercontent.com/91744454/220844436-da81903b-c26a-4720-bb03-5db610c13a52.png)
![imagen](https://user-images.githubusercontent.com/91744454/220844468-21391345-d94e-4302-a07d-227d60650672.png)
![imagen](https://user-images.githubusercontent.com/91744454/220844585-92b46779-df80-4a03-ace2-f139468623a9.png)
![imagen](https://user-images.githubusercontent.com/91744454/220844607-067b7e73-4402-471f-83df-02f613005c88.png)

La fuente que he utilizado en este proyecto es "Poppins", de google-fonts.

Como podemos observar tiene una barra de navegación principal y una página de inicio donde debería haber un carrousel (no se me renderizaba bien y por falta de tiempo he tenido que quitarlo)  

Tenemos una sección donde se cargarán las notas. Como podemos comprobar aún no tenemos ninguna nota:  

![imagen](https://user-images.githubusercontent.com/91744454/220838974-5ad10572-8811-40df-a850-4b9462a0ced7.png)

![imagen](https://user-images.githubusercontent.com/91744454/220839074-327454cd-516f-4ab6-95b6-75151dfb1a82.png)

Para empezar a escribir notas, solo tenemos que iniciar la api que tenemos en el propio repositorio.  

![imagen](https://user-images.githubusercontent.com/91744454/220839727-2571c4d8-ca17-4602-96f9-191f6d569971.png)

Al darle al botón 'crear nota' nos redirige a un formulario donde podemos escribirla.  
![imagen](https://user-images.githubusercontent.com/91744454/220839884-68e0956f-36f8-4ee9-8d9a-b48894076a9f.png)

Como podemos observar, se ha creado:  

![imagen](https://user-images.githubusercontent.com/91744454/220840003-b91f7467-9f8d-4238-b45d-7800abd38ce3.png)

Vamos a probar de editarla:  

![imagen](https://user-images.githubusercontent.com/91744454/220840048-b15b96ef-ff4c-457f-97c7-84369b61fd3c.png)

Vemos que nos lleva a un formulario al cual le hemos pasado por parámetro las propiedades de la nota.   

![imagen](https://user-images.githubusercontent.com/91744454/220840152-8c90d5f3-7746-4b18-b7ac-4a690f68eb7a.png)

Al darle a actualizar, mediante el método PUT actualiza nuestra base de datos.  


![imagen](https://user-images.githubusercontent.com/91744454/220840362-9dc6f054-801d-4215-bf47-7455c4fff982.png)

Como podemos observar en la pantalla superior derecha, nos aparece un mensaje pop-up avisándonos de que la actualización se ha realizado con éxito. 

Este mensaje (toast) lo he programado mediante mixins.  

(https://user-images.githubusercontent.com/91744454/220842270-7f426742-4ff1-4f8e-a7c3-fda8e1a26278.png)


Luego sencillamente se importa en el componente que necesite lanzar el pop-up:  
![imagen](https://user-images.githubusercontent.com/91744454/220842863-a6c6edfa-2d5a-42a9-bfa1-5a3ad928801f.png)


![imagen](https://user-images.githubusercontent.com/91744454/220842838-a64476e0-a2cf-4be6-8a09-051623a4f055.png)

No tiene mucha más complicación.  

Si en vez de actualizar la nota queremos eliminarla, solo tenemos que darle al botón.


![imagen](https://user-images.githubusercontent.com/91744454/220840584-b10cff4d-4cee-4d43-8848-b009a2162ff3.png)

He tenido un problema con el renderizado y por lo tanto, al eliminar una nota se elimina con normalidad pero no actualiza la página. Es necesario actualizarla manualmente.  

![imagen](https://user-images.githubusercontent.com/91744454/220840747-84c59172-1703-42f3-acd6-df0609283aa3.png)  


A parte de las funcionalidades Create, Read, Update, Delete, habia creado un apartado para buscar notas a partir de su Id:  


![imagen](https://user-images.githubusercontent.com/91744454/220840786-ce65f197-3111-412f-b2a4-1c294b90e316.png)

La realidad ha sido que me ha sido imposible hacer una función para que me haga un fetch(id), ya que no se por qué funcionaba sólo a la segunda vez de apretar el botón (la primera vez me devolvía un array vacío) y por tanto no podía pasar nada por parámetro. No he podido arreglarlo por falta de tiempo.

Al poner la pantalla modo móvil, podemos comprobar que es responsiva:  

![imagen](https://user-images.githubusercontent.com/91744454/220841493-3b62e7ab-4fdf-4941-a021-26e7f0195bdf.png)

Al apretar el botón hamburguesa se despliega un menú:  

![imagen](https://user-images.githubusercontent.com/91744454/220841559-f6850be0-3367-45c6-b8cb-a47091e72a67.png)

Creamos una nota desde el móvil y...  


![imagen](https://user-images.githubusercontent.com/91744454/220841651-04baab62-f284-425d-ba65-b079d9c438eb.png)


## Project setup
```
npm install
```

### Compiles and hot-reloads for development
```
npm run serve
```

### Compiles and minifies for production
```
npm run build
```

### Lints and fixes files
```
npm run lint
```

### Customize configuration
See [Configuration Reference](https://cli.vuejs.org/config/).
