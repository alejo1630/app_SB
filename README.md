# 📊 Análisis de la App **Bolívar Conmigo**

Este repositorio contiene el desarrollo del **caso de negocio analítico** solicitado por Seguros Bolívar, enfocado en el análisis de la aplicación **Bolívar Conmigo** y la identificación de factores asociados a la **inactividad de los usuarios**, con el fin de proponer estrategias para mejorar la retención y el uso activo de la app.

---

## 📌 Contexto del Proyecto
Seguros Bolívar lanzó la app **Bolívar Conmigo** con el objetivo de:
- Mejorar la calidad de vida de sus usuarios promoviendo un estilo de vida saludable.  
- Proteger la salud, el bienestar, los vehículos y el hogar de los clientes.  
- Ofrecer acompañamiento en momentos clave de la vida.  

La aplicación está disponible para clientes y no clientes de Seguros Bolívar.

Sin embargo, se identificó un **alto número de usuarios inactivos** pese al crecimiento en registros. Este análisis busca comprender las causas de dicha inactividad y proponer soluciones basadas en datos.

---

## 📂 Estructura de Datos

Se trabajó con dos fuentes principales (archivo `Datos_Caso_2025.xlsx`):
1. **Datos Demográficos**  
   - Género, estado civil, ingresos, actividad económica, número de hijos.  
   - Productos de seguros contratados: salud, vida, autos.  

2. **Datos de Interacciones**  
   - Fechas de interacción, tipo de interacción (registro, workout, survey, points, inactivo, etc.).  
   - Canal y plataforma de interacción.  

---

## 🔎 Metodología de Análisis

1. **Exploratory Data Analysis (EDA)**  
   - Limpieza de valores nulos, duplicados y unificación de categorías.  
   - Análisis de distribuciones: edad, ingresos, estado civil, productos de seguros.  
   - Visualización de patrones de interacción y grupos de edad.  

2. **Cruce de Datasets**  
   - Identificación de **usuarios huérfanos** (presentes en interacciones pero no en demográficos).  
   - Filtrado de interacciones no asociadas a la app (correo, chatbot).  

3. **Modelado Estadístico**  
   - Regresión logística para estimar la probabilidad de que un usuario sea **activo/inactivo** en función de variables demográficas y de interacción.  
   - Cálculo de **odds ratios** para interpretar la relevancia de cada factor.  

---

## 📈 Hallazgos Principales

- **Usuarios huérfanos**: 8.05% de usuarios y 5.89% de interacciones no tienen correspondencia entre bases.  
- **Edad**: Los usuarios más jóvenes (20–29 años) presentan mayor inactividad (≈58%).  
- **Género**: Los hombres son más propensos a la inactividad (43%) frente a las mujeres (36%).  
- **Actividad económica**: Los empleados concentran gran parte de los inactivos (43%).  
- **Productos de seguros**: A mayor número de productos contratados, mayor probabilidad de inactividad.  
- **Interacciones**: Muchos usuarios se vuelven inactivos tras encuestas (survey) o registros iniciales.  

---

## 💡 Estrategias Propuestas

1. **Gamificación y recompensas**  
   - Incentivos para mantener actividad posterior al registro y encuestas.  
   - Retos personalizados según grupo de edad.

2. **Segmentación de campañas**  
   - Campañas específicas para hombres jóvenes y empleados (segmentos más inactivos).  
   - Mensajes personalizados para usuarios con múltiples productos de seguros.  

3. **Optimización del Onboarding**  
   - Mejorar la experiencia inicial tras registro y survey para evitar abandono temprano.  

4. **Monitoreo de cohortes**  
   - Seguimiento mensual de tasas de actividad por edad, género y actividad económica.  

---

## 🛠️ Tecnologías Utilizadas
- **Python** (pandas, numpy, matplotlib, seaborn, statsmodels, scipy)  
- **Jupyter Notebook** para análisis y visualización interactiva  
- **Excel** como fuente de datos inicial  


---

## 📢 Autor
**Alejandro Castellanos Vargas**  
Data Scientist | Machine Learning | Analítica de Negocios  
