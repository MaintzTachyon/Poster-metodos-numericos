# Figuras del póster

La columna 3 de `poster_NACA0018.tex` ya incluye las figuras 2–5. Las imágenes
definitivas se extrajeron directamente del PDF del informe
(`referencia/MN_P2_Grupo_1.pdf`) para conservar la mayor resolución disponible.

## Archivos en uso

| Figura | Archivo            | Contenido                                      | Tamaño (px) |
|--------|--------------------|------------------------------------------------|-------------|
| 2      | `figura2.png`      | Equilibrios estáticos e histéresis (paneles a y b) | 1010 × 673 |
| 3      | `figura3.png`      | Respuesta dinámica del caso base               | 985 × 639   |
| 4      | `figura4.png`      | Efecto de la frecuencia                        | 1031 × 681  |
| 5      | `figura5.png`      | Contraste con datos digitalizados              | 1011 × 681  |

Las imágenes son las incrustadas originalmente en el PDF del informe; no son
capturas de pantalla, por lo que no hay pérdida adicional por reescalado.

En `figura2.png` se eliminó el título recortado del panel derecho (el informe
lo trae cortado en el borde). El panel izquierdo conserva su título.

## Imágenes de respaldo

- `originales_whatsapp/`: fotos enviadas por WhatsApp (251–466 px de ancho).
  Son de muy baja resolución para impresión; se conservan solo como referencia.
- `figura1_convergencia_no_usar.png`: figura 1 del informe (orden de
  convergencia). No se usa en el póster.
- `figura2a_equilibrios_x.png`, `figura2b_equilibrios_cn.png`,
  `figura3_respuesta_dinamica.png`, `figura4_efecto_frecuencia.png`,
  `figura5_contraste_datos.png`: copias renombradas de las fotos de WhatsApp.
  No se usan en la versión actual.

## Cómo se insertan

La figura 2 ocupa media columna con su propio bloque; las figuras 3, 4 y 5 usan
el comando `\figimage{archivo}{número}{pie}{alto máximo}` definido al inicio
del `.tex`. Ejemplo:

```latex
\figimage{Figuras/figura3.png}{3}%
  {Evolución temporal del estado y trayectorias del ciclo base en función
   del ángulo de ataque.}{12cm}
```

El ancho de cada figura es el de media columna (18.05 cm) y la altura se ajusta
respetando la proporción original.

## Logo

`logo_utec.png` se extrajo de la portada del informe `MN_P2_Grupo_1.pdf`.
Si tienes el logo oficial en mayor resolución, reemplaza este archivo
manteniendo el nombre o actualiza la ruta en la banda superior del `.tex`.
