# Ingeniería de Requerimientos (ISR-401)

Repositorio personal de **Vaca Romero David Octavio** de la carrera de Ingeniería de Software, Universidad Técnica Estatal de Quevedo. Las actividades están organizadas en carpetas independientes.

## FORM-TL-01: Identificación y clasificación de tipos de requisitos

**Estado:** versión con clasificación E01–E20, cinco requisitos de calidad cuantificados y contraste documental con el repositorio de Angelo Espinoza. **El contraste documental no demuestra una conversación ni un acuerdo bilateral**, y la revisión académica del estudiante sigue siendo necesaria.

**Caso:** Plataforma de gestión de citas médicas (material del docente).

### Estructura de archivos

- `FORM-TL-01/main.tex`: fuente principal del documento académico.
- `FORM-TL-01/main.pdf`: PDF compilado del documento académico (NO es el PDF que se entrega directamente al SGA).
- `FORM-TL-01/secciones/requisitos.tex`: clasificación en tres dimensiones y justificación E01–E20.
- `FORM-TL-01/secciones/calidad.tex`: reformulación cuantificada de E03, E07, E10, E14 y E18.
- `FORM-TL-01/secciones/discrepancias.tex`: contraste documental con el trabajo de Angelo Espinoza, diferencias verificadas y decisiones técnicas argumentadas. No se declara una discusión oral o un acuerdo entre ambos.
- `FORM-TL-01/secciones/enunciados.tex`: enunciados proporcionados por el docente.
- `FORM-TL-01/portada_sga.tex`: fuente de la portada informativa.
- `FORM-TL-01/portada_sga.pdf`: carátula de una página con la URL del repositorio para subir al SGA.

### Compilar los PDF

**Compilador:** pdfLaTeX (`pdflatex`), por ejemplo con TeX Live o MiKTeX. Paquetes necesarios: `babel` (español), `fontenc`, `inputenc`, `lmodern`, `geometry`, `array`, `longtable`, `booktabs`, `tabularx`, `xcolor`, `microtype`, `hyperref` y `enumitem`.

Desde la raíz del repositorio, ejecutar en este orden:

```bash
cd FORM-TL-01
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error portada_sga.tex
```

**Alternativa sin instalar LaTeX:** importar la carpeta `FORM-TL-01` completa en Overleaf, seleccionar `main.tex` como archivo principal, compilar con pdfLaTeX y descargar el PDF. El PDF descargado debe colocarse en `FORM-TL-01/main.pdf` del repositorio.

### Revisión antes de entregar

1. Revisar cada clasificación y las características/subcaracterísticas ISO/IEC 25010:2023 frente a las fuentes disponibles.
2. Revisar las cinco métricas como propuestas de aceptación, no presentarlas como acuerdos ni mediciones reales.
3. Revisar el contraste documental con el trabajo de Angelo Espinoza y, si se realiza un diálogo adicional, registrar por separado los acuerdos que efectivamente se alcancen.
4. Verificar la declaración de apoyo de IA en `main.tex`, las fuentes y la comparación antes de presentarla como propia.
5. Regenerar `main.pdf` **después de la última modificación** de cualquier archivo `.tex`, publicarlo y comprobar que coincide con el contenido de la fuente.
6. Revisar que `portada_sga.pdf` tenga exactamente una página y que la URL escrita en ella sea accesible.

**Entrega SGA:** subir únicamente `FORM-TL-01/portada_sga.pdf` (una página, menor de 1 MB), una vez terminado y actualizado el repositorio. Según el registro del SGA compartido, la fecha límite es 7 de noviembre de 2026, 23:59 (Ecuador). La guía PDF original contiene una fecha y modalidad distintas; confirmar cualquier cambio oficial del docente.

Los commits deben describir cambios reales y verificables; no simular historial de trabajo.

### Evidencia de comparación documental

Se contrastó la clasificación individual con la fuente facilitada del repositorio de Angelo: https://github.com/Espinoza-A-1006/ISR401-EspinozaAngelo (copia ZIP compartida el 7 de noviembre de 2026). Se detectaron diferencias principales en **E02** y **E09**, un matiz en **E10** y un umbral alternativo para **E14**. Las decisiones explicadas en el PDF son criterios académicos propuestos por David, **no acuerdos ni conversaciones atribuidos a Angelo**. La fuente de Angelo duplicaba E03 y E04 en su `main.tex`; fueron comparados una sola vez.
