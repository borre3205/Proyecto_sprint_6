# Sprint 6 — Análisis de ventas de videojuegos 🎮

## 📋 Descripción del proyecto

Análisis exploratorio de datos para la tienda online **Ice**, que vende videojuegos en todo el mundo. El objetivo es identificar patrones que determinen si un juego tiene éxito o no, permitiendo detectar proyectos prometedores y planificar campañas publicitarias para 2017.

El análisis utiliza datos históricos de ventas de videojuegos por plataforma, género, región y reseñas de críticos y usuarios, con datos que cubren el período relevante de **2011 a 2016**.

## 🎯 Preguntas de negocio respondidas

- ¿Qué plataformas son líderes en ventas y cuáles están en declive?
- ¿Cómo afectan las reseñas de críticos y usuarios a las ventas?
- ¿Qué géneros son más rentables por región?
- ¿Existen diferencias en las preferencias de los usuarios por región (NA, EU, JP)?
- ¿Las clasificaciones ESRB afectan las ventas en distintas regiones?

## 🔍 Estructura del análisis

- **Paso 1**: Carga y revisión general de los datos
- **Paso 2**: Preparación y limpieza de datos (valores ausentes, tipos de datos, TBD)
- **Paso 3**: Análisis exploratorio de datos
  - Ciclo de vida de plataformas
  - Definición del período de análisis (2011-2016)
  - Boxplots de ventas por plataforma
  - Correlación reseñas vs ventas
  - Análisis de juegos multiplataforma
  - Distribución de ventas por género
- **Paso 4**: Perfil de usuario por región (NA, EU, JP)
  - Top 5 plataformas por región
  - Top 5 géneros por región
  - Impacto de clasificación ESRB por región
- **Paso 5**: Prueba de hipótesis
  - Calificaciones promedio de XOne vs PC
  - Calificaciones promedio de Acción vs Deportes
- **Paso 6**: Conclusión general

## 📊 Hallazgos clave

- El ciclo de vida típico de una consola es de **7-8 años**, lo que justifica el período de análisis 2011-2016.
- **PS4 y XOne** son las plataformas con mayor potencial para 2017, seguidas de **3DS** y **PC**.
- La **calificación de críticos** tiene una correlación moderada con las ventas (0.40), mientras que la **calificación de usuarios** prácticamente no tiene relación (-0.03).
- **PS4 duplica las ventas** del promedio de sus competidores para los mismos títulos multiplataforma (0.88M vs 0.44M).
- **Shooter** es el género con mayor promedio de ventas por título (1.22M).
- **NA y EU** comparten preferencias similares (PS4, Shooter, clasificación M), mientras **JP** tiene un perfil muy distinto (3DS, Role-Playing, clasificación NE).
- No hay diferencia significativa entre las calificaciones de usuarios de XOne y PC (p=0.61).
- Sí hay diferencia significativa entre las calificaciones de Acción y Deportes (p≈5.8×10⁻¹⁹).
<img width="580" height="478" alt="imagen(2)" src="https://github.com/user-attachments/assets/957b0753-d3b0-4485-906c-340c1167e7d0" />
<img width="1229" height="702" alt="imagen(1)" src="https://github.com/user-attachments/assets/d6e509c5-6ccf-4287-999d-bd8bbec9682d" />
<img width="1218" height="1240" alt="imagen" src="https://github.com/user-attachments/assets/c4ff5665-3e60-459c-b281-a00a232c4f36" />

## 🛠️ Stack técnico

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- SciPy

## 📁 Estructura del proyecto
sprint6-videogames-analysis/

├── README.md

├── requirements.txt

├── games.ipynb

└── games.csv

## ▶️ Cómo ejecutar localmente

```bash
# Clonar el repositorio
git clone https://github.com/borre3205/sprint6-videogames-analysis.git
cd sprint6-videogames-analysis

# Crear y activar entorno virtual
python -m venv venv
.\venv\Scripts\activate  # Windows
source venv/bin/activate  # Mac/Linux

# Instalar dependencias
pip install -r requirements.txt

# Abrir el notebook
jupyter notebook games.ipynb
```

## 👤 Autor
Santiago Quintanilla — Mechatronics Engineer | Data Science Student @ TripleTen
[LinkedIn](https://www.linkedin.com/in/santiago-quintanilla-zurita-b5117b103) | [GitHub](https://github.com/borre3205)
