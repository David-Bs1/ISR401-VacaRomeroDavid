# Ingeniería de Requerimientos (ISR-401)

Repositorio académico personal de **Vaca Romero David Octavio**, estudiante de Ingeniería de Software de la **Universidad Técnica Estatal de Quevedo (UTEQ)**.

**Asignatura:** Ingeniería de Requerimientos (ISR-401)  
**Nivel y paralelo:** Cuarto nivel, Software A  
**Docente:** PhD. Gleiston Cicerón Guerrero Ulloa

## Actividades del repositorio

| Actividad | Tema y caso de estudio | Documentos |
|---|---|---|
| **FORM-TL-01** | Identificación y clasificación de 20 enunciados de requisitos. Caso: plataforma de gestión de citas médicas. Incluye requisitos de calidad cuantificados y contraste documental. | [Informe](FORM-TL-01/main.pdf) · [Fuente LaTeX](FORM-TL-01/main.tex) · [Portada SGA](FORM-TL-01/portada_sga.pdf) |
| **TA-IND-01 / TA-TAR-01** | Análisis de ISO/IEC/IEEE 29148:2018 y tipos de requisitos de **Spotify**. Incluye glosario, 15 requisitos, autoevaluación y tres capturas propias. | [Guía de la actividad](TA-IND-01/README.md) · [Informe](TA-IND-01/main.pdf) · [Fuente LaTeX](TA-IND-01/main.tex) · [Portada SGA](TA-IND-01/portada_sga.pdf) |

Cada actividad se guarda en una carpeta independiente. Los archivos `.tex` son las fuentes editables; los archivos `.pdf` corresponden a las versiones compiladas. Las portadas del SGA son distintas de los informes académicos completos.

## Estructura

```text
ISR401-VacaRomeroDavid/
├── .gitignore
├── README.md
├── FORM-TL-01/
│   ├── main.tex
│   ├── main.pdf
│   ├── portada_sga.tex
│   ├── portada_sga.pdf
│   └── secciones/
└── TA-IND-01/
    ├── README.md
    ├── main.tex
    ├── main.pdf
    ├── referencias.bib
    ├── portada_sga.tex
    ├── portada_sga.pdf
    ├── figuras/
    └── secciones/
```

## Compilación reproducible

Se necesita una distribución **TeX Live** o **MiKTeX** con **pdfLaTeX**; para TA-IND-01 también se requiere **Biber** y `biblatex`. Se deben instalar los paquetes LaTeX utilizados en los preámbulos de cada `main.tex` (entre ellos `babel` para español, `geometry`, `longtable`, `graphicx` y `hyperref`).

Desde la raíz del repositorio, ejecutar los comandos correspondientes a la actividad.

### FORM-TL-01

```bash
cd FORM-TL-01
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error portada_sga.tex
```

### TA-IND-01

```bash
cd TA-IND-01
pdflatex -interaction=nonstopmode -halt-on-error main.tex
biber main
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error main.tex
pdflatex -interaction=nonstopmode -halt-on-error portada_sga.tex
```

Para ejecutar ambos bloques en una misma terminal, regresar antes a la raíz del repositorio (`cd ..`). El detalle de dependencias, evidencias y límites de la actividad de Spotify está documentado en **[TA-IND-01/README.md](TA-IND-01/README.md)**.

## Evidencias e integridad académica

- **FORM-TL-01:** el contraste con otro repositorio es documental; no se presenta como un diálogo o acuerdo bilateral.
- **TA-IND-01:** las tres capturas de Spotify fueron aportadas por el estudiante. Los umbrales de calidad son **criterios de aceptación propuestos**, no resultados de pruebas realizadas.
- Las fuentes, declaraciones de apoyo con IA y limitaciones deben revisarse en los documentos de cada actividad. El historial de Git debe describir cambios reales.

## Entrega en el SGA

Para cada actividad, el SGA solicita únicamente su **portada informativa de una página**, con la dirección completa y pública de este repositorio en una sola línea. El informe, sus fuentes y las evidencias permanecen en GitHub.

**Repositorio:** https://github.com/David-Bs1/ISR401-VacaRomeroDavid
