# TA-IND-01 — Análisis de requisitos de Spotify

**Asignatura:** Ingeniería de Requerimientos (ISR-401) · **Modalidad:** individual.  
**Sistema estudiado:** Spotify para escritorio · **Normas:** ISO/IEC/IEEE 29148:2018 e ISO/IEC 25010:2023.

## Contenido

- `main.tex` — archivo principal del informe; incorpora módulos de `secciones/` igual que la actividad FORM-TL-01.
- `main.pdf` — PDF completo compilado.
- `referencias.bib` — bibliografía verificable (formato IEEE).
- `figuras/` — tres imágenes originales aportadas por el estudiante.
- `portada_sga.tex` y `portada_sga.pdf` — ficha informativa de **una página** para el SGA.

## Reproducción

Se requiere una distribución TeX Live o MiKTeX con `pdflatex`, `biber`, `biblatex`, `babel-spanish`, `geometry`, `longtable`, `hyperref` y los paquetes indicados en el preámbulo de `main.tex`. El compilador utilizado para el informe fue **pdfLaTeX** con `biber`.

Desde la carpeta `TA-IND-01/` (sin sobrescribir otras actividades del repositorio):

```bash
pdflatex -interaction=nonstopmode -halt-on-error main.tex
biber main
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error portada_sga.tex
```

El README indica el orden de los comandos: la primera pasada genera la información de citas, `biber` procesa la bibliografía y las dos pasadas finales actualizan referencias, índices y numeración de figuras.

## Evidencias incluidas (sin edición visual)

| Archivo | Evidencia visible | Límites |
|---|---|---|
| `figuras/busqueda_spotify.png` | Búsqueda del término “Human” y resultados | No mide el tiempo de respuesta |
| `figuras/playlist_spotify.png` | Playlist personal “Mi lista n.º 1” con 3 canciones | No documenta todos los pasos de creación |
| `figuras/sesion_privada_spotify.png` | Opción “Sesión privada” en el menú de perfil | No demuestra activación ni eficacia del ocultamiento |

Las capturas son material de primera mano aportado por el estudiante en esta conversación. Las métricas R-11 a R-15 son **propuestas de aceptación no medidas**. No se fabricaron entrevistas, participantes, ensayos ni resultados.

## Integridad académica y revisión necesaria

El proyecto contiene un **borrador elaborado con apoyo de ChatGPT (OpenAI, GPT-6)**, declarado en el informe. Su uso debe ajustarse a las instrucciones del docente. El estudiante debe verificar las citas y cláusulas, revisar los 15 requisitos, adaptar con su propia experiencia la reflexión y poder explicar o corregir el documento sin apoyo; la declaración no convierte automáticamente el texto generado en autoría propia. No se deben inventar commits pasados ni otras evidencias.

## Entrega

En GitHub debe quedar la carpeta `TA-IND-01/` completa, sin reemplazar `FORM-TL-01/` ni otras actividades. Este paquete incluye el repositorio anterior intacto y un apartado nuevo en su README raíz. En el SGA se sube **solamente `TA-IND-01/portada_sga.pdf`**, nunca el informe de varias páginas ni el ZIP. Verifique previamente que el enlace del repositorio sea público y que la URL aparezca en una sola línea.

**Repositorio de referencia proporcionado previamente:** https://github.com/David-Bs1/ISR401-VacaRomeroDavid  
**Fecha límite actualizada comunicada en clase:** 11 de noviembre de 2026, 23:59 (hora Ecuador).
