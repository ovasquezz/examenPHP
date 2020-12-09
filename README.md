# examenPHP
 
(Para empezar tenego un error que no he corregido aún en la pagina de read_one.php pero aunque no se muestre los cambios que he hecho deberian ser correctos)

4- Para poner el simbolo dolar al lado del precio he editado los arachivos read_template.php y read_one.php que son los encargados de escribir los datos en la tabla, cuando va a printar el precio, he añadido \$ antes de la variable del precio para ponerlo como caracter y lo imprima en todas las filas

5- El usuario elige una imagen y el programa llama a la funcion uploadPhoto() que se encarga de comprobar que la imagen cumple los siguientes requisitos:

- Si es una imagen de verdad.
- Si la imagen es del formato correcto, en nuestro caso tiene que ser "jpg", "jpeg", "png" o "gif".
- Que la imagen no supere 1MB de peso.
- Que la imagen no exista, es decir, que no exista otro producto con la misma imagen

Si la imagen cumple con todos los requisitos se guarda en una carpeta llamada /uploads que se crea automaticamente si no tenemos una ya creada de nuestro proyecto y en la gase de datos, que tiene que estar configurada como un VARCHAR de una longitud de 512.

Para recuperarla selecciona la imagen correspondiente al objeto seleccionado y busca su ruta en la carpeta /uploads, si la encuentra la muestra, si no aparece un error en pantalla diciendo que no se encuentra la imagen. 

6- Para actualizar una imagen he utilizado el mismo principio que para crearla, he añadido la propiedad imagen al objeto product en el archivo update_product.php y cuando intente actualizar el producto llamando a la funcion update(), tambien llamara a la funcion updatePhoto(), que es igual que uploadPhoto() que utilizamos para crear un producto. La diferencia que tiene updatePhoto() es que no importa si ya hay un producto con la misma imagen ya que de ser asi no nos dejaria actualizarla.

Además, en la tabla de update_products.php he añadido el selector de archivos para que pueda elegir la foto para actualizar.



He añadido un archivo para configurar la base de datos.