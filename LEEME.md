# Póster — Histéresis aerodinámica NACA 0018

Archivos principales:

| Archivo | Descripción |
|---|---|
| `poster_NACA0018.tex` | Fuente LaTeX del póster (48 × 36 pulgadas, horizontal). |
| `poster_NACA0018.pdf` | Póster compilado, listo para revisar o imprimir. |
| `poster_NACA0018_preview.png` | Vista previa rápida en imagen. |
| `Figuras/logo_utec.png` | Logo UTEC extraído de la portada del informe. |
| `Figuras/figura2.png` … `figura5.png` | Figuras 2–5 del informe, extraídas del PDF. |
| `Figuras/LEEME.md` | Detalle de las figuras, respaldos y resolución. |

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
- **Columna 3:** figuras 2–5, sensibilidad, contraste con datos, alcance,
  conclusiones y referencias.

## Figuras

Las figuras 2–5 ya están insertadas y provienen del PDF del informe
(`referencia/MN_P2_Grupo_1.pdf`), no de las fotos de WhatsApp, para garantizar
la mejor calidad de impresión. Revisa `Figuras/LEEME.md` para ver los nombres,
tamaños y respaldos.
