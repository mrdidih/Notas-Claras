# Nota Clara 🎓

Una calculadora gratuita de notas universitarias, sin anuncios, sin cuentas y sin dependencias. Puedes usarla en el computador, iPad o celular.

## Funciones

- Crear, editar y eliminar materias.
- Registrar evaluaciones con porcentajes y notas (las notas pendientes se dejan en blanco).
- Calcular el acumulado y el promedio de las evaluaciones calificadas.
- Calcular el promedio mínimo necesario en el porcentaje restante para aprobar.
- Personalizar la nota de aprobación y la nota máxima de la escala.
- Guardar materias automáticamente en el almacenamiento local del **navegador de cada dispositivo**.
- Exportar e importar copias de seguridad en formato JSON.

### Ejemplo

| Evaluación | Peso | Nota |
| --- | ---: | ---: |
| Primer corte | 30 % | 4,2 |
| Segundo corte | 30 % | 3,8 |
| Examen final | 40 % | Pendiente |

Acumulado: `4,2 × 0,30 + 3,8 × 0,30 = 2,40`.

Para aprobar con 3,0, falta un promedio de `(3,0 - 2,4) / 0,40 = 1,50` en el 40 % pendiente.

## Uso local

Abre `index.html` en un navegador. No requiere instalación, servidor, Node ni acceso a internet para calcular notas.

**Importante:** los datos son independientes en cada dispositivo y navegador. No se suben a GitHub ni se sincronizan. Al borrar los datos del navegador, cambiar de navegador o pasar del archivo local al sitio publicado, los registros no se trasladan automáticamente: usa **Guardar copia** y luego **Cargar copia**.

## Publicar gratis con GitHub Pages

1. Crea un repositorio público en GitHub, por ejemplo `nota-clara`.
2. Sube `index.html`, `README.md` y `.nojekyll` a la **raíz** del repositorio, en la rama `main` (sin ponerlos dentro de una carpeta adicional).
3. En el repositorio abre **Settings → Pages**.
4. En **Build and deployment → Source**, elige **Deploy from a branch**; selecciona `main` y `/(root)`, y pulsa **Save**.
5. Abre el enlace que muestre GitHub Pages. Si el usuario es `mrdidih` y el repositorio `nota-clara`, la dirección habitual sería `https://mrdidih.github.io/nota-clara/` (solo funcionará una vez publicado).

Si subes la aplicación desde un ZIP, **descomprímelo primero**: GitHub Pages no ejecuta un archivo ZIP directamente.

## Tecnología

Un solo archivo HTML con CSS y JavaScript, sin frameworks ni servicios externos. Usa `localStorage` para guardar información.

## Privacidad

El repositorio público aloja únicamente el **código de la aplicación y notas ficticias de ejemplo**. Las materias reales que ingreses se guardan solo en el navegador donde las escribas. Recomendamos descargar copias de seguridad de vez en cuando.
