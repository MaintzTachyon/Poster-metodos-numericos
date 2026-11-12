# Figuras del póster

En la columna 3 del archivo `poster_NACA0018.tex` hay cuatro espacios reservados
para las figuras 2–5 del informe. Cada espacio tiene el tamaño definitivo que
ocupará la imagen, de modo que el diseño no se desplazará al insertarlas.

## Nombres sugeridos

Guarda las imágenes en esta carpeta con estos nombres:

| Figura | Archivo sugerido      | Contenido                                      |
|--------|-----------------------|------------------------------------------------|
| 2      | `figura2.png`         | Equilibrios estáticos e histéresis             |
| 3      | `figura3.png`         | Respuesta dinámica del caso base               |
| 4      | `figura4.png`         | Efecto de la frecuencia                        |
| 5      | `figura5.png`         | Contraste con datos digitalizados              |

Se recomienda PNG a 300 dpi o PDF vectorial exportado desde el informe.

## Cómo insertar una figura

En el archivo `.tex`, localiza el bloque `\figslot{2}{...}{...}` y reemplaza
toda la llamada por:

```latex
\begin{minipage}[t]{18.05cm}
  \centering
  \includegraphics[width=\linewidth,height=11.2cm,keepaspectratio]{Figuras/figura2.png}\\[0.24cm]
  {\captionfont\textbf{Figura 2.} Variable de separación $x$ y coeficiente
   $C_N$: ramas estables, rama inestable y puntos de pliegue.\par}
\end{minipage}%
```

Haz lo mismo con las figuras 3, 4 y 5. El comando `\figslot` está definido al
inicio del archivo, junto con el ancho (18.05 cm) y el alto (11.2 cm) de cada
espacio.

## Logo

`logo_utec.png` se extrajo de la portada del informe `MN_P2_Grupo_1.pdf`.
Si tienes el logo oficial en mayor resolución, reemplaza este archivo
manteniendo el nombre o actualiza la ruta en la banda superior del `.tex`.
