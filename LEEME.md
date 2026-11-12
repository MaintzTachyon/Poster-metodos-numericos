# Póster — Histéresis aerodinámica NACA 0018

Archivos principales:

| Archivo | Descripción |
|---|---|
| `poster_NACA0018.tex` | Fuente LaTeX del póster (48 × 36 pulgadas, horizontal). |
| `poster_NACA0018.pdf` | Póster compilado, listo para revisar o imprimir. |
| `poster_NACA0018_preview.png` | Vista previa rápida en imagen. |
| `Figuras/logo_utec.png` | Logo UTEC extraído de la portada del informe. |
| `Figuras/LEEME.md` | Instrucciones para insertar las figuras 2–5. |

## Compilación

Se compila con **pdfLaTeX** (no requiere XeLaTeX):

```bash
pdflatex poster_NACA0018.tex
pdflatex poster_NACA0018.tex
```

La segunda pasada es necesaria para estabilizar los elementos `overlay` de TikZ
(bandas superior e inferior).

## Distribución

- **Columna 1:** introducción, objetivos, pregunta de investigación y
  metodología (diagrama de flujo).
- **Columna 2:** sistema de ecuaciones, parámetros del modelo y resultados
  principales (equilibrios, respuesta dinámica y comparación de métodos).
- **Columna 3:** espacios para las figuras 2–5, sensibilidad, contraste con
  datos, alcance, conclusiones y referencias.

## Figuras pendientes

Los cuatro espacios de la columna 3 ya tienen el tamaño definitivo. Sigue
`Figuras/LEEME.md` para reemplazarlos por las imágenes del informe sin alterar
la maquetación.
