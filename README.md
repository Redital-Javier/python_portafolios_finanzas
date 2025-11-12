# 🐍 python_portafolios_finanzas  
**Simulación de carteras moderada y agresiva con Python.**  
Análisis de riesgo, frontera eficiente y métricas de performance aplicadas a una cartera diversificada de acciones, ETFs sectoriales y criptoactivos (2022–2025).

---

## 🎯 Objetivo del proyecto
Este proyecto tiene como propósito aplicar los conceptos del curso **Python para Finanzas** a un caso práctico de inversión, simulando distintas estrategias para un inversor con **perfil moderado**.  
Se busca identificar portafolios eficientes mediante análisis cuantitativo, utilizando métricas de riesgo y rendimiento.

---

## 🧱 Estructura del análisis

El estudio se desarrolla paso a paso dentro de la notebook principal:

### **📊 Parte 1 – Selección y descarga de datos**
- Selección de **12 activos diversificados**: acciones estadounidenses, latinoamericanas, ETFs sectoriales y un criptoactivo (Bitcoin).  
- Descarga de precios históricos (enero 2022 – junio 2025) mediante `yfinance`.  
- Limpieza y preparación del dataset.

### **🔍 Parte 2 – Análisis exploratorio**
- Evolución de precios ajustados e índices normalizados (base 100).  
- Cálculo de retornos diarios y medidas de volatilidad.  
- Histogramas, boxplots y matriz de correlación.  
- Clasificación de activos según su perfil: **defensivos, equilibrados o agresivos**.

### **⚙️ Parte 3 – Métricas de riesgo y retorno**
- Cálculo de **Betas (CAPM)** para medir exposición al mercado.  
- Ratios de **Sharpe**, **Sortino** y **Treynor** para evaluar eficiencia ajustada por riesgo.  
- Aplicación del modelo **Fama-French 3 factores**, analizando la sensibilidad de cada activo a los factores de mercado, tamaño y valor.

### **💼 Parte 4 – Simulación de portafolios**
- Simulación tipo Monte Carlo con **10.000 combinaciones aleatorias de pesos**.  
- Identificación del portafolio de **Máxima Sharpe** y de **Mínima Volatilidad**.  
- Visualización de la **frontera eficiente** y comparación de composiciones.  
- Evaluación del rendimiento acumulado (2022–2025).

### **🧭 Parte 5 – Conclusiones y recomendaciones**
- Síntesis comparativa entre ambas estrategias.  
- Recomendaciones según distintos perfiles de riesgo.  
- Limitaciones metodológicas y posibles mejoras futuras.

---

## 📈 Resultados destacados

| Estrategia | Retorno anual | Volatilidad | Sharpe | Retorno acumulado | Capital final |
|-------------|----------------|--------------|---------|--------------------|----------------|
| 🚀 Máxima Sharpe | **38.76%** | 25.22% | **1.54** | 242.94% | \$3.43 |
| 🧘‍♂️ Mínima Volatilidad | 7.27% | **15.79%** | 0.46 | 23.15% | \$1.23 |

**Conclusión:**  
- El portafolio de **Máxima Sharpe** prioriza el crecimiento, asumiendo más volatilidad.  
- El de **Mínima Volatilidad** ofrece estabilidad con retornos moderados, ideal para inversores prudentes.  
Ambos representan estrategias viables para un perfil **moderado**, según el balance deseado entre rentabilidad y riesgo.

---

## 🧩 Tecnologías y librerías utilizadas

| Tipo | Librería | Uso principal |
|------|-----------|---------------|
| Datos | `pandas`, `numpy`, `yfinance` | Descarga y manipulación de series históricas |
| Visualización | `matplotlib`, `seaborn` | Gráficos de precios, correlaciones y composiciones |
| Modelado | `statsmodels` | CAPM y Fama-French (regresiones lineales) |
| Optimización | `numpy`, simulación Monte Carlo | Generación de 10.000 portafolios |
| Estadística financiera | `PyPortfolioOpt` *(opcional)* | Alternativa para frontera eficiente |

---

📘 Proyecto desarrollado como Trabajo Final del curso *Python para Finanzas* (2025).


