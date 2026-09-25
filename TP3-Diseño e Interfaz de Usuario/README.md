# Trabajo Practico: HTML y CSS
Licenciatura en Sistemas de Informacion - Diseno UX-UI (2026)

## Ejercicios resueltos

Se resolvieron los 20 ejercicios del TP, organizados en carpetas separadas
(`ejercicio-01` a `ejercicio-20`), cada una con su propio `index.html` y,
a partir del Ejercicio 5 (donde se introduce el CSS externo), tambien su
`styles.css`.

| Bloque | Ejercicios | Tema |
|---|---|---|
| 1 - Basico | 1 a 4 | HTML puro: estructura, listas/enlaces, tablas, formularios |
| 1 - Basico | 5 a 7 | Primer CSS, selectores, box model |
| 2 - Intermedio | 8 a 14 | Flexbox, Grid, pseudo-clases/elementos, posicionamiento, formularios estilizados, variables CSS |
| 3 - Medio/avanzado | 15 a 20 | Responsive, animaciones, menu hamburguesa sin JS, grid mosaico, formulario multi-step, proyecto integrador |

## Decisiones de diseño

- **Ejercicios 1 a 4 sin CSS**: siguiendo la progresion del TP (el CSS se
  introduce recien en el Ejercicio 5, que pide "aplicar un CSS externo a la
  pagina del Ejercicio 1"), esas cuatro primeras carpetas contienen solo
  HTML. Del Ejercicio 5 en adelante cada carpeta tiene su `styles.css`.
- **Hilo conductor "Chipas ER"**: varios ejercicios (listas, tabla de
  horarios, galerias de productos, landing final) usan como contenido real
  el negocio de venta de chipas, en lugar de lorem ipsum, para que el TP
  quede mas cerca de un caso real y reutilizable.
- **Ejercicio 15**: se justifico un enfoque *desktop first* (se parte del
  layout completo del Ejercicio 10 y se lo va simplificando con media
  queries), en linea con lo que ya estaba armado en Grid.
- **Ejercicio 19**: el multi-step se resolvio con el truco de radio buttons
  ocultos + selector `~` (sin `:target` ni JavaScript), y la validacion
  visual usa `:invalid` / `:valid` combinados con `:not(:placeholder-shown)`
  para no marcar los campos en rojo antes de que el usuario escriba.
- **Ejercicio 20**: integra Flexbox (navbar, formulario) y Grid (galeria de
  productos) en el mismo sitio, variables CSS globales, dos media queries
  (900px y 600px), una unica animacion de entrada en el hero (siguiendo el
  criterio de usar la animacion en un solo momento, no repetida en cada
  tarjeta) y HTML semantico (`header`, `main`, `section`, `footer`). El CSS
  esta dividido en secciones numeradas y comentadas.
- Las imagenes usan `picsum.photos` como placeholder, ya que no se contaba
  con fotos propias para el repositorio.
