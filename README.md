# 🚀 Predicción de Satisfacción Cliente con Gradient Boosting 😊
![satisfacion](https://image.lexica.art/full_webp/0d685497-d8ef-4acc-95e6-636cc5c00302)

¡Bienvenido al repositorio de modelos avanzados para experiencia de cliente! Este proyecto utiliza **Gradient Boosting (XGBoost, LightGBM, CatBoost)** para predecir el nivel de satisfacción de clientes basado en interacciones de servicio. Ideal para centros de contacto, retail y empresas de servicios.

## 📋 Tabla de Contenidos
1. [Requisitos](#🔧-requisitos)
2. [Instalación](#⚙️-instalación)
3. [Uso](#🚀-uso)
4. [Estructura del Proyecto](#📂-estructura-del-proyecto)
5. [Datos](#📊-datos)
6. [Resultados](#📈-resultados)
7. [Contribución](#🤝-contribución)
8. [Licencia](#📜-licencia)
9. [Contacto](#📧-contacto)

---

## 🔧 Requisitos
- Python 3.8+
- Bibliotecas: `xgboost`, `lightgbm`, `catboost`, `pandas`, `scikit-learn`, `shap`
- GPU (opcional, para entrenamiento acelerado)

## ⚙️ Instalación
```bash
# Clonar repositorio
git clone https://github.com/tuusuario/gb-satisfaccion-cliente.git

# Instalar dependencias
pip install -r requirements.txt

# Instalación opcional para GPU
pip install --upgrade xgboost lightgbm catboost --install-option=--cuda
```
## 📂 Estructura del Proyecto
├── data/  
│   ├── satisfaccion_clientes.csv    # Dataset principal  
│   └── generador_datos.py           # Generador de datos sintéticos  
├── modelos/  
│   ├── comparacion_gb.py            # Comparación XGBoost/LightGBM/CatBoost  
│   ├── optimizacion.py              # Optimización hiperparámetros  
│   └── interpretacion_shap.py       # Explicabilidad del modelo  
├── notebooks/  
│   ├── EDA_satisfaccion.ipynb       # Análisis exploratorio interactivo  
│   ├── comparacion_modelos.ipynb    # Benchmark de algoritmos  
│   └── analisis_shap.ipynb          # Interpretación con SHAP  
├── resultados/  
│   ├── shap_summary.png             # Importancia global  
│   ├── dependencia_tiempo_espera.png# Gráficos de dependencia  
│   ├── mejor_modelo.cbm             # Modelo optimizado serializado  
│   └── metricas_comparativas.csv    # Resultados comparativos  
└── requirements.txt 

## 📊 Datos   
- Variables del dataset ficticio (generado sintéticamente):

- tiempo_espera (Minutos en espera)

- interacciones (Número de contactos requeridos)

- edad (Edad del cliente)

- tipo_servicio (Categórico: Técnico, Facturación, Ventas, Soporte)

- canal (Teléfono, Chat, Email, Presencial)

- resolucion_primer_contacto (Binario: Sí/No)

- Target: satisfaccion (Puntuación 1-100)

## 🤝 Contribución
¡Tu experiencia es valiosa! Contribuye mediante:

- Reporte de bugs o sugerencias en Issues

- Mejora de documentación

- Optimización de hiperparámetros

- Nuevos análisis de interpretación
  
##📜 Licencia  
Distribuido bajo licencia Apache 2.0. Ver LICENSE para detalles.

¡Si te gusto dame una estrella! 🚀
