def# Escribe el problema de tu 01-perfil.md como te lo pediría un jefe o cliente
• Tradúcelo a una pregunta que los datos puedan responder y a la decisión que
apoya
• ¿Qué datos necesitarías? ¿Cuáles tienes, cuáles faltan y qué habría que
transformar?
• ¿Qué tipo de tarea es?

## 1. El problema desde la perspectiva del jefe o cliente
> *"Necesito saber cuánto vamos a vender las próximas semanas"*

---

## 2. Traducción a preguntas

* **Pregunta que los datos pueden responder:** 
  ¿Cuál es el volumen de ventas esperado por producto para los próximos 7, considerando el numero de asistentes, estrenos y promociones?
* **Decisión que apoya:** 
  Optimizar el reabastecimiento de inventario en almacén, evitando tanto el desabasto como el exceso y planificar la asignación operativa de personal según la demanda esperada.

---

## 3. Requerimientos de datos 

* **¿Qué datos necesitaría?**
  * Histórico de transacciones diarias, cantidad vendida por producto.
  * Niveles actuales de inventario.
  * Número de asistentes al día.
  * Asistencia esperada para ese periodo
  * Promociones disponibles y futuras 

* **¿Cuáles tengo actualmente?**
  * Registros de fecha y hora de las transacciones, monto, cantidad en stock, cantidad vendida.
  * Número de asistentes por semana 

* **¿Cuáles faltan?**
  * Promociones disponibles y futuras
  * Asistentes proyectados para la semana

* **¿Qué habría que transformar?**
  * **Limpieza y estandarización:** Limpiar datos con duplicados o fallas de captura, decidir com lidiar con mermas y faltantes.
  * **Agrupació:** Agrupar por items vendidos y dias de la semana.
  * **Ingeniería de características (*Feature Engineering*):** Extraer datos como asistentes esperados y % de afluencia por días.

---

## 4. ¿Qué tipo de tarea de Ciencia de Datos es?
Es un problema de Regresión, ya que el objetivo es predecir ventas futuras a partir de datos historicos.