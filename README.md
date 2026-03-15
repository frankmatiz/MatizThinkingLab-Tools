# Simulador de Inversiones — MATIZ Leadership & Thinking Lab

Herramienta interactiva para comparar dos inversiones con interés compuesto, métricas avanzadas y análisis con recomendación automática.

## ¿Qué incluye?

- Comparación lado a lado de dos inversiones configurables
- Gráfica de crecimiento en el tiempo (Chart.js)
- Tabla comparativa con indicadores por categoría
- Métricas avanzadas: CAGR, tiempo para duplicar capital, multiplicador de valor
- Análisis y veredicto automático generado localmente (sin API key)
- Branding MATIZ integrado
- 100% frontend — un solo archivo HTML, sin dependencias externas

## Cómo usar

Abre el link de GitHub Pages y empieza a configurar:

1. Escribe el nombre de cada inversión
2. Ajusta capital inicial, aporte mensual, tasa anual, plazo y capitalización
3. Presiona **"Generar análisis y recomendación"** para obtener el veredicto

## Parámetros disponibles

| Campo | Rango |
|---|---|
| Capital inicial | $500 – $200,000 |
| Aporte mensual | $0 – $5,000 |
| Tasa anual | 0% – 30% |
| Plazo | 1 – 40 años |
| Capitalización | Anual / Mensual / Diaria |

## Modelo financiero

El cálculo usa **tasa efectiva mensual** derivada de la frecuencia de capitalización elegida, simulando mes a mes para mantener consistencia entre el capital inicial y los aportes periódicos.

```
tasa_mensual_efectiva = (1 + tasa_anual / n)^(n/12) - 1
balance_mes = balance_anterior × (1 + tasa_mensual) + aporte_mensual
```

## Aviso

Este simulador es de uso **educativo**. Los resultados proyectados asumen tasas constantes y no constituyen asesoría financiera profesional.

---

© MATIZ – Leadership & Thinking Lab · Todos los derechos reservados
