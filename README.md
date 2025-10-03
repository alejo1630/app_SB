# Análisis de la App **Bolívar Conmigo**

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

- **Simplificar el flujo de registro y encuesta**, reduciendo pasos y tiempo.  
- **Incentivos inmediatos** tras completar encuestas o registro.  
- Personalizar notificaciones **con base en intereses más comunes**.  
- Promover el uso de la app en **horarios no laborales** con notificaciones personalizadas favoreciendo las **microinteracciones**.  
- Ofrecer **beneficios corporativos** (alianzas con empresas y planes colectivos).  
- Unificar información de todos los seguros de una forma **simple** para reducir fricción.  
- **Programas de fidelización**: a mayor número de productos contratados, **más beneficios digitales**.  
- Crear campañas digitales enfocadas en el segmento **20–29 años** (Instagram, TikTok).  
- **Gamificación**: retos y recompensas que generen **sensación de logro**.  
- **Notificaciones inteligentes**: no solo recordatorios, sino mensajes de valor (“Tu plan te protege en viajes”, “Gana puntos extra esta semana”).  
- Implementar **pruebas A/B** para optimizar la efectividad de flujos, campañas y notificaciones antes de su despliegue masivo.  

---

## 🛠️ Tecnologías Utilizadas
- **Python** (pandas, numpy, matplotlib, seaborn, statsmodels, scipy)  
- **Jupyter Notebook** para análisis y visualización interactiva  
- **Excel** como fuente de datos inicial  



