# Simulación y Procesos Estocásticos — TP1
### Probabilidad, Estadística y Generación de Números Aleatorios

**Pontificia Universidad Católica Argentina — Licenciatura en Ciencias de Datos**  
Año 2026

---

##  Descripción

Trabajo práctico grupal que aborda los fundamentos teóricos y computacionales de la simulación estocástica, desde la caracterización de distribuciones de probabilidad hasta la generación y verificación de números pseudoaleatorios en Python.

---

##  Contenido del repositorio

| Archivo | Descripción |
|---|---|
| `TP1_Simulacion_2026.ipynb` | Notebook con implementaciones y visualizaciones |
| `TP1_Simulacion_Informe.pdf` | Informe completo en formato académico |

---

##  Temas cubiertos

### 1. Distribuciones estadísticas
Caracterización de 7 distribuciones con fórmulas, escenarios de aplicación y visualizaciones:
- **Continuas:** Uniforme, Triangular, Exponencial, Normal
- **Discretas:** Bernoulli, Binomial, Poisson

### 2. Generación de números pseudoaleatorios
- **Método de los Cuadrados Medios** (von Neumann, 1946): implementación y análisis de dependencia con la semilla
- **Generador Congruencial Lineal (LCG):** implementación con parámetros Lewis-Learmonth ($M = 2^{31}-1$, $a = 16807$, $c = 0$)

### 3. Variantes del método congruencial
Implementación y comparación de:
- Congruencial **Multiplicativo** ($c = 0$)
- Congruencial **Aditivo** ($a = 1$)
- Congruencial **Mixto** (caso general)

### 4. Pruebas de aleatoriedad
Implementación de 7 tests estadísticos para verificar uniformidad e independencia:
- Prueba Chi-cuadrado
- Prueba de Kolmogorov-Smirnov (KS)
- Prueba de Autocorrelación
- Prueba de la Corrida (Runs Test)
- Prueba de Repetitividad
- Prueba de Uniformidad de los Dígitos
- Prueba de Distancia

### 5. Transformada inversa
Generación de variables aleatorias con distribución arbitraria a partir de $U \sim U[0,1]$:
- Exponencial: $X = -\ln(U)/\lambda$
- Uniforme$(a,b)$: $X = a + (b-a) \cdot U$
- Triangular (fórmula general)
- Distribuciones discretas (Bernoulli, Poisson)

---

##  Tecnologías utilizadas

![Python](https://img.shields.io/badge/Python-3.11-blue?logo=python)
![NumPy](https://img.shields.io/badge/NumPy-1.26-blue?logo=numpy)
![Matplotlib](https://img.shields.io/badge/Matplotlib-3.8-blue)
![SciPy](https://img.shields.io/badge/SciPy-1.11-blue?logo=scipy)
![Jupyter](https://img.shields.io/badge/Jupyter-Notebook-orange?logo=jupyter)

```python
import numpy as np
import matplotlib.pyplot as plt
from scipy import stats
```

---

##  Cómo ejecutar

1. Clonar el repositorio:
```bash
git clone https://github.com/choco721/Pseudorandom-generators-from-scratch.git
cd Pseudorandom-generators-from-scratch
```

2. Instalar dependencias:
```bash
pip install numpy matplotlib scipy
```

3. Abrir el notebook:
```bash
jupyter notebook TP1_Simulacion_2026.ipynb
```

---

##  Autores

- Chocobares, Juan Cruz
- Formenti, Agustín


---

##  Referencias

- Ross, S. M. (2023). *Simulation*, 6th Edition. Academic Press.
- Banks, J. et al. (1996). *Discrete-Event System Simulation*. Prentice Hall.
- Ciaburro, G. (2022). *Hands-On Simulation Modeling with Python*, 2nd Edition. Packt.
