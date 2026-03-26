# 📈📊Evaluación de la Calidad de Tendencia con Volatilidad y SMA

## 📌Descripción del proyecto

Este proyecto implementa una consulta SQL para evaluar la calidad de una tendencia de precios, combinando información de media móvil (SMA) y volatilidad.

El objetivo es clasificar las tendencias no solo por su dirección (alcista o bajista), sino también por su consistencia, estabilidad y nivel de riesgo, permitiendo distinguir entre:
- Tendencias sólidas
- Tendencias débiles
- Movimientos erráticos o ruidosos

## 🎯Objetivos del proyecto

- Calcular medias móviles (SMA) como referencia de tendencia.
- Medir la volatilidad asociada al movimiento de precios.
- Evaluar la calidad de la tendencia en el tiempo.
- Detectar deterioros o mejoras en la estructura del movimiento.
- Automatizar análisis técnico avanzado mediante SQL.

## 🏦Contexto financiero

No todas las tendencias son iguales:
- Una tendencia con baja volatilidad suele ser más confiable.

Tendencias con alta volatilidad pueden indicar:
- Riesgo elevado
- Movimientos especulativos
- Falta de convicción del mercado

📌 Evaluar la calidad de la tendencia permite:

- Mejorar timing de entrada y salida
- Gestionar riesgo
- Evitar señales falsas
- Optimizar estrategias cuantitativas

## 🧠Lógica del análisis

La consulta SQL:
- Ordena precios en el tiempo.
- Calcula la SMA como referencia direccional.
- Calcula métricas de volatilidad.

Evalúa:
- Dirección del precio respecto a la SMA
- Consistencia del movimiento
- Nivel de ruido
- Clasifica la tendencia, por ejemplo:
- Fuerte
- Moderada
- Débil
- Errática

📌 Los parámetros son configurables según activo y horizonte temporal.

## 📊Ejemplos de insights

- Tendencias alcistas con baja volatilidad → alta calidad.
- Tendencias con frecuentes cruces de la SMA → baja calidad.
- Incrementos de volatilidad que anticipan ruptura de tendencia.
- Cambios graduales en la calidad antes de una reversión.

## 🛠️Tecnologías utilizadas

SQL

Compatible con:
- PostgreSQL
- BigQuery
- SQL Server
- Oracle
- MySQL (con ajustes menores)

## 📁Estructura del proyecto

├── Calidad_tendencia_Volatilidad_SMA.sql
└── README.md

## ▶️Cómo utilizar la consulta

Abrir el archivo Calidad_tendencia_Volatilidad_SMA.sql.

Configurar:
- Tabla de precios
- Ventana de SMA
- Métrica de volatilidad
- Ejecutar la consulta en el motor SQL.
- Integrar resultados en análisis, dashboards o alertas.

## 🚀Posibles extensiones

- Incorporar múltiples SMAs o EMAs.
- Medir estabilidad de la tendencia en distintas ventanas.
- Combinar con volumen u otros indicadores técnicos.
- Generar alertas de deterioro de tendencia.
- Integrar con modelos predictivos.

## 👤Autora

Flavia Hepp
Proyecto de SQL aplicado a análisis técnico y evaluación de calidad de tendencia.

****
📈⚠️ **Buenas noticias… pero una tendencia “sucia” — algo no cierra**

En teoría, cuando una empresa anuncia una recompra de acciones, el mensaje es claro:

👉 Confianza de la gerencia
👉 Señal positiva al mercado

Pero… el precio no siempre acompaña de forma “saludable”.

---

💡 Estuve analizando un insight interesante:

**¿Qué pasa cuando el precio está demasiado alejado de su tendencia de largo plazo (SMA 200) justo en estos eventos?**

---

🔥 **La señal que buscamos:**

* 🟢 Evento positivo → recompra de acciones
* 📊 Pero el precio está a más de **5% de su SMA 200**
* ⚠️ Indica una **desviación significativa** respecto a la tendencia

---

🧠 **¿Qué significa esto?**

No todo rally es “limpio”.

👉 Puede haber:

* Volatilidad excesiva
* Sobre-reacción del mercado
* Movimientos poco sostenibles

---

📉 En otras palabras:

Aunque la señal fundamental sea positiva…
👉 la estructura técnica puede estar mostrando **fragilidad**

---

📊 ¿Por qué es importante?

Porque permite filtrar:

* ❌ Señales “ruidosas”
* ✅ Tendencias realmente sólidas

---

⚡ Aplicaciones:

* Evaluar calidad de tendencias post-evento
* Evitar entradas en zonas extendidas
* Mejorar timing en estrategias long
* Detectar posibles correcciones

---

💬 No todas las buenas noticias generan buenos trades.

👉 La clave no es solo el “qué”…
sino el **cómo se mueve el precio alrededor de su tendencia**

---

En trading cuantitativo, la calidad del movimiento importa tanto como la dirección.

¿Preferís entrar en tendencias limpias… o perseguir movimientos fuertes aunque sean volátiles? 👇
