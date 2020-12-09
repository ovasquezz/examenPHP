# examenPHP
 
(Para empezar tenego un error que no he corregido aún en la pagina de read_one.php pero aunque no se muestre )

4- Para poner el simbolo dolar al lado del precio he editado los arachivos read_template.php y read_one.php que son los encargados de escribir los datos en la tabla, cuando va a printar el precio, he añadido \$ antes de la variable del precio para ponerlo como caracter y lo imprima en todas las filas

5- El usuario elige una imagen y el programa llama a la funcion uploadPhoto() que se encarga de comprobar que la imagen cumple los siguientes requisitos:

- Si es una imagen de verdad.
- Si la imagen es del formato correcto, en nuestro caso tiene que ser "jpg", "jpeg", "png" o "gif".
- Que la imagen no supere 1MB de peso.
- Que la imagen no exista, es decir, que no exista otro producto con la misma imagen

Si la imagen cumple con todos los requisitos se guarda en una carpeta llamada /uploads que se crea automaticamente si no tenemos una ya creada de nuestro proyecto y en la gase de datos, que tiene que estar configurada como un VARCHAR de una longitud de 512.

Para recuperarla selecciona la imagen correspondiente al objeto seleccionado y busca su ruta en la carpeta /uploads, si la encuentra la muestra, si no aparece un error en pantalla diciendo que no se encuentra la imagen. 

6-



He añadido un archivo para configurar la base de datos.