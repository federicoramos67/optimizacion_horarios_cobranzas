# 📞 Optimización de horarios de llamadas en gestión de mora

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/12KOPp6kIrTvwpUpG7kl0fCmyaegorjdn)

## 🎯 Resumen ejecutivo

Sistema de recomendación de horarios óptimos para contactar clientes en gestión de mora temprana y tardía mediante análisis de datos históricos.

**Reducción proyectada:** llamadas improductivas mediante priorización inteligente de contactos.

---

## 📊 El problema

En centros de contacto especializados en cobranzas:
- **~55% de llamadas no son atendidas**
- Los clientes evitan el contacto o no están disponibles
- Tiempo operador desperdiciado en horarios de baja efectividad
- Ausencia de criterio basado en datos para priorizar contactos

**Costo empresarial:** baja tasa de contacto efectivo, menor recuperación de mora.

---

## ✨ La solución

Análisis predictivo de patrones de atención telefónica:

✅ **Identificación** de mejores franjas horarias por cliente  
✅ **Priorización** de contactos por probabilidad de atención  
✅ **Recomendaciones accionables** para equipos operativos  
✅ **Métricas de impacto** cuantificables

---

## 🚀 Demo interactiva

**[▶️ Ejecutar notebook en Google Colab](https://colab.research.google.com/github/[TU-USUARIO]/optimizacion-horarios-cobranzas/blob/main/demo_optimizacion_llamadas_visual.ipynb)**

*No requiere instalación. Usa datos sintéticos. Totalmente privado.*

---

## 📈 Resultados generados

El análisis produce:

### 1. Tabla de mejores horarios por cliente
Identifica la franja óptima basada en histórico de atención

### 2. Ranking de contactos prioritarios
Top clientes con mayor probabilidad de respuesta

### 3. Plan de acción operativo
Distribución de llamadas por franjas horarias del día

### Ejemplo de salida:

```
🎯 PLAN DE LLAMADAS OPTIMIZADO
=========================================

✅ Cliente 1004
   → Llamar en: NOCHE (18:00 - 21:00 hs)
   → Probabilidad de atención: 71%
   → Basado en 7 intentos previos

✅ Cliente 1010
   → Llamar en: MAÑANA (08:00 - 12:00 hs)
   → Probabilidad de atención: 60%
   → Basado en 5 intentos previos

✅ Cliente 1006
   → Llamar en: NOCHE (18:00 - 21:00 hs)
   → Probabilidad de atención: 50%
   → Basado en 6 intentos previos
```

---

## 🛠️ Stack técnico

- **Python 3.8+**
- **Pandas** - manipulación y agregación de datos
- **NumPy** - generación de datos sintéticos

---

## 📋 Metodología

### Fase 1: Simulación de datos
Generación de 250 registros históricos:
- 10 clientes
- 25 intentos de contacto por cliente
- Distribución realista de resultados (35% atención, 55% no atención, 10% rechazo)

### Fase 2: Feature engineering
- Segmentación de horarios en franjas: Mañana (08-12h), Tarde (12-18h), Noche (18-21h)
- Variable binaria de atención efectiva

### Fase 3: Análisis agregado
- Cálculo de tasas de atención por cliente y franja
- Identificación de mejor horario individual

### Fase 4: Generación de recomendaciones
- Ranking de contactos prioritarios
- Plan de acción con asignación horaria

---

## 💡 Insights demostrados

Este proyecto muestra:

- **Pensamiento analítico:** transformación datos → decisiones
- **Orientación al negocio:** problema real → solución medible
- **Reproducibilidad técnica:** código limpio, documentado, ejecutable
- **Comunicación clara:** explicable para stakeholders técnicos y no técnicos

---

## 🔄 Escalabilidad productiva

Este proof of concept puede extenderse a:

- ✅ Integración con bases de datos reales (MySQL/PostgreSQL)
- ✅ Procesamiento de millones de registros
- ✅ Ejecución automática nocturna (cron jobs)
- ✅ Exportación a CRM o sistemas de discado automático
- ✅ Dashboard interactivo con Streamlit/Plotly
- ✅ Segmentación por tipo de mora (temprana/tardía)
- ✅ Análisis por día de la semana

---

## 📁 Estructura del notebook

| Sección | Descripción |
|---------|-------------|
| **Celda 1** | Contexto del problema en gestión de mora |
| **Celdas 2-3** | Stack técnico e importaciones |
| **Celdas 4-5** | Generación de dataset sintético (250 registros) |
| **Celdas 6-7** | Feature engineering y transformación |
| **Celdas 8-9** | Análisis agregado y cálculo de tasas |
| **Celdas 10-11** | Identificación de mejores horarios |
| **Celdas 12-13** | Métricas de impacto empresarial |
| **Celdas 14-15** | Plan de acción operativo priorizado |
| **Celda 16** | Conclusiones y próximos pasos |

---

## 🔐 Privacidad y ética

- Datos 100% sintéticos generados con `numpy.random`
- No expone información real de clientes
- Ejecución local sin envío de datos externos
- Replicable con `seed(42)` para reproducibilidad

---

## 📝 Licencia

MIT License - Libre uso con atribución

---

## 👤 Autor

**Federico ramos**

- 🔗 LinkedIn: https://www.linkedin.com/in/federicoramosf/
- 💻 GitHub: https://github.com/federicoramos67
- 📧 Email: federicoramos6767@gmail.com

---

## 🤝 Contribuciones

¿Mejoras o ideas? Abrí un issue o pull request.

---

**⭐ Si este proyecto te resultó útil, dejá una estrella en GitHub**
