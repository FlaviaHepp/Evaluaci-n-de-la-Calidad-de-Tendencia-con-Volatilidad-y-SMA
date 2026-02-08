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
