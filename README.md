# Prediccion del Rendimiento Academico con Machine Learning

Proyecto academico de Machine Learning supervisado que responde dos preguntas:

1. **Clasificacion:** ¿el alumno aprobara o reprobara?
2. **Regresion:** ¿cual sera la calificacion final del alumno?

## Contenido

```text
Proyecto_MachineLearning/
├── Dataset/
│   ├── alumnos.csv
│   └── diccionario_datos.csv
├── Clasificacion/
│   └── clasificacion.ipynb
├── Regresion/
│   └── regresion.ipynb
├── Imagenes/
│   └── graficas y evidencias.png
├── Documentacion/
│   ├── Reporte.pdf
│   ├── Reporte.docx
│   └── resultados_modelos.json
├── README.md
├── requirements.txt
└── GUIA_GITHUB.md
```

## Dataset

- 200 registros sinteticos y anonimos.
- 7 variables predictoras.
- Variable objetivo de clasificacion: `Resultado`.
- Variable objetivo de regresion: `Calificacion_Final`.
- No contiene valores faltantes ni registros duplicados.

## Modelos

| Problema | Modelo inicial | Modelo optimizado |
|---|---|---|
| Clasificacion | Decision Tree Classifier | Random Forest Classifier + GridSearchCV |
| Regresion | Decision Tree Regressor | Random Forest Regressor + GridSearchCV |

## Resultados principales

### Clasificacion

- Accuracy antes: **0.700**
- Accuracy despues: **0.825**
- F1 despues: **0.851**

### Regresion

- RMSE antes: **9.243** puntos
- RMSE despues: **5.873** puntos
- R2 despues: **0.716**

## Herramientas

Python, Pandas, NumPy, Scikit-Learn, Matplotlib, Jupyter/Google Colab, Excel/CSV y GitHub.

## Ejecucion en Google Colab

1. Sube el proyecto a GitHub.
2. Abre el notebook deseado desde GitHub con Google Colab.
3. Clona el repositorio en una celda o sube `alumnos.csv` al entorno de Colab.
4. Ejecuta **Entorno de ejecucion > Ejecutar todas**.

Ejemplo para clonar:

```python
!git clone URL_DE_TU_REPOSITORIO
%cd NOMBRE_DEL_REPOSITORIO/Proyecto_MachineLearning/Clasificacion
```

## Ejecucion local

```bash
pip install -r requirements.txt
jupyter notebook
```

Luego abre `Clasificacion/clasificacion.ipynb` o `Regresion/regresion.ipynb` y ejecuta todas las celdas.

> Nota: la instalacion local es opcional si se utiliza Google Colab.

## Integrantes

- [Escribe aqui los nombres de los integrantes]

## Consideracion etica

El dataset es sintetico. Un sistema real debe validar sesgos, proteger datos personales y usar las predicciones como apoyo, no como sustituto de la evaluacion humana.
