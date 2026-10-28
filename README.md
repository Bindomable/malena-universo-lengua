# Malena · Universo Lengua

Aplicación estática en español para estudiar los apuntes de Lengua de Malena. Funciona en móvil, tableta y ordenador, sin instalar dependencias ni usar servicios de IA o cuentas de alumnado.

## Contenido

- 31 fichas: comunicación, seis tipos de textos, literatura y géneros, y doce figuras literarias.
- Preguntas de conceptos y casos originales con identificación y razonamiento.
- Práctica por bloques, repaso de errores, reto final de 20 preguntas equilibradas, notas, XP e insignias.
- El mito se define exactamente como «Es una narración literaria».
- Se aclara que la prosa es una forma de escritura y que tipo de texto, género y figura son ejes distintos. La clasificación de derivación sigue los apuntes.

## Publicación en GitHub Pages

1. Sube `index.html`, `styles.css`, `content.js`, `app.js` y `.nojekyll` a la raíz de un repositorio.
2. En Settings → Pages elige Deploy from a branch, rama `main`, carpeta `/ (root)`.
3. Abre la dirección que GitHub indique. Todos los recursos usan rutas relativas, por lo que funcionan bajo el nombre de un repositorio.

No hay compilación. Puedes abrir `index.html` directamente para una prueba rápida; para guardar progreso de manera estable utiliza la URL de GitHub Pages.

## Progreso y puntuaciones

El navegador conserva la sesión en curso, lecturas, resultados, errores, conceptos dominados, puntos e historial en `localStorage`. No se envían datos del alumnado a ningún servidor y no existe sincronización automática. El progreso pertenece al dispositivo, navegador y origen web; cambiar de dirección puede cambiar el almacenamiento. «Guardar copia» y «Recuperar copia» permiten trasladarlo en JSON; la importación vuelve al inicio y conserva resultados, pero no reanuda una pregunta a medias.

Cada ficha aporta 5 XP una vez; cada paso de pregunta correcto aporta 10 XP una vez. Los fallos no restan XP. Una pregunta práctica tiene dos pasos y solo se considera superada cuando ambos son correctos en el mismo intento. Un concepto requiere dos preguntas diferentes superadas, al menos una práctica. La nota de una misión es la proporción de pasos correctos multiplicada por 10. La nota del reto no equivale al dominio de todos los conceptos.

El reto se puede repetir e incluye corrección durante su realización: sirve para autoevaluación formativa. Se muestran los diez resultados más recientes y se conservan hasta cincuenta.

## Editar

El contenido está en `content.js`; comportamiento y puntuaciones en `app.js`; diseño adaptable en `styles.css`. Los ejemplos son originales y están basados en los conceptos de las cinco páginas aportadas. Una página del PDF repetía las figuras literarias. No se publican las fotografías del cuaderno.
