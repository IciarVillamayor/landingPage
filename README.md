IMPORTANTE PARA ALUMNOS

A) INICIO
Si no está la carpeta node_modules/ en la raíz, es por que no hemos instalado
las dependencias todavía 
- Abrimos la terminal (Ver terminal)
- Escribimos npm install

B) EMPEZAR A FUNCIONAR
- Escribimos npm run dev
- Y vamos a nuestro navegador y ponemos la URL http://127.0.0.1:5500

C) CORTAR LA COMPILACIÓN
Le damos a Ctrl +  C (la gente que tiene Mac tb, Ctrl no Cmd)

D) Añadir nuevas dependencias (jQuery, u otras librerías)
- Cortamos la compilación (mirar C)
- Ponemos npm install NOMBRE_DE_MI_LIBRERIA_A_INSTALAR --save
- Ejemplo: npm install jquery --save 
- Otro ejemplo: npm install flickity --save
- Importamos en ./app/index.js nuestra librería (tenemos un ejemplo allí)
- Volvemos a ejecutar (Mirar B)

E) Añadir nueva página estática (si es necesario)
- En la carpeta pages/, hago un archivo nuevo por ejemplo mipagina.ejs
- En el archivo webpack.config.js (con mucho cuidado) en la línea 45 tengo un ejemplo de como
hacer una página nueva.

F) Para entregar
- Borro la carpeta node_modules/
- Comprimo la carpeta y le pongo mi nombre
- Subo la entrega al aula

G) El Emmet no me funciona en los archivos EJS
- Vamos al JSON de preferencias: Ctrl (o Cmd) + Shift + P y escribimos "settings.json"
- Le damos a user settings
- Escribimos al final antes del cierre de la última llave:
  "emmet.includeLanguages": {
    "ejs": "html"
  }