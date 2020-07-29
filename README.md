En producción, se recomienda minimizar cualquier código JavaScript que se incluya con la aplicación. La minificación puede ayudar a su sitio web a cargarse varias veces más rápido, especialmente a medida que aumenta el tamaño del código fuente de JavaScript.

Aquí hay una manera de configurarlo:

[Instalar Node.js](https://nodejs.org/)
Ejecutar `npm init -y` en la carpeta del proyecto(**no omita este paso!npm init**)
Ejecutar `npm install terser`
Ahora, para minimizar un archivo llamado `example.js`, ejecute en el terminal o la línea de comandos

```
npx terser -c -m -o example.min.js -- like_button.js
```
Esto generará un archivo llamado `example.min.js` con el código minificado en el mismo directorio. Si escribe esto con frecuencia, puede crear un script npm para asignar un nombre a este comando.
