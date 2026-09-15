# Terminal de Predicción Binance

## 📊 Descripción

Terminal web interactiva para predicción direccional de precios de criptomonedas en Binance.

**Versión:** v6 (núcleo verificado, purga y auditoría en hilo secundario)

## 🎯 Características

- ✅ Predicción en tiempo real (modo en vivo y replay histórico)
- ✅ Análisis técnico con 5 factores de decisión
- ✅ Auditoría estadística completa (PBO, Sharpe deflactado, DSR)
- ✅ Validación de datos y reconciliación entre proveedores
- ✅ Gestión de riesgo y cartera simulada
- ✅ Walk-forward y multi-horizonte
- ✅ Calibración de confianza (curva de calibración)
- ✅ Glosario de 90+ términos

## 🚀 Cómo usar

1. Abre `terminal-prediccion-v6.html` en tu navegador
2. Selecciona un par (BTC/USDT, ETH/USDT, etc.)
3. Configura temporalidad y horizonte
4. Pulsa **Iniciar** para comenzar análisis

## ⚙️ Modos de operación

- **Replay histórico** (rápido): Simula sobre datos históricos
- **En vivo por WebSocket** (real): Streaming en tiempo real de Binance

## 📈 Proveedores de datos

- Binance REST API
- Binance Vision
- OKX
- Bybit
- Coinbase

## 📋 Parámetros

### Parámetros de hecho (no cuentan como ensayo)
- Comisión por lado (pbs)
- Horquilla modelada (pbs)
- Pago binario (%)
- Capital simulado (€)

### Parámetros de modelo (cuentan como ensayo)
- Umbral de operación
- EMA rápida y lenta
- Periodo RSI
- Retroceso de momento
- Ventana y peso de canal
- Pesos de tendencia, momento, fuerza relativa y reversión

## 🔍 Auditoría estadística

La terminal ejecuta:
- **CSCV**: Validación cruzada combinatoria por bloques
- **PBO**: Probabilidad de sobreajuste del backtest
- **DSR**: Sharpe deflactado (con corrección Newey-West)
- **Walk-forward**: Estabilidad temporal
- **Permutación**: Test contra hipótesis nula

## 📊 Secciones

- **Conexión y parámetros**: Configuración del sistema
- **Diagnóstico de red**: Pruebas de conectividad
- **Gráfico**: Visualización de velas y predicciones
- **Predicción**: Probabilidades en tiempo real
- **Auditoría**: Análisis estadístico completo
- **Riesgo y cartera**: Simulación de saldo
- **Contexto y agenda**: Eventos determinísticos del mercado
- **Laboratorio**: Walk-forward y multi-horizonte

## ⚠️ Importante

- **Modo demo**: Las predicciones aquí no son reales
- **Sin recomendación financiera**: Esto es una herramienta educativa
- **Validación requerida**: Audita sobre datos nuevos antes de operar capital real
- **Costo real**: Incluye spread y comisiones en todos los cálculos

## 🛠️ Tecnología

- HTML5 Canvas para gráficos
- WebSocket para datos en vivo
- Web Workers para auditoría en hilo secundario
- IndexedDB para caché local
- API REST de Binance y otros exchanges

## 📄 Licencia

MIT - Libre para usar, modificar y distribuir

## 🤝 Contribuciones

Las contribuciones son bienvenidas. Por favor:
1. Fork el repositorio
2. Crea una rama (`feature/mejora`)
3. Commit tus cambios
4. Push y abre un Pull Request

## 📞 Soporte

Para reportar errores o sugerencias, abre un Issue en el repositorio.

---

**Última actualización:** 2026-09-15