# 🔥 CS2 Trading Bot - Sistema de Consola

Sistema simplificado de trading automático para skins de CS2 usando DMarket API.

## 🚀 Características

- ✅ Trading REAL con dinero real (no simulación)
- 📊 Análisis de mercado en tiempo real
- 🎯 Estrategias de trading automatizadas
- 💰 Seguimiento de KPIs y ROI
- 🔍 Detección de oportunidades de arbitraje
- 📦 Gestión de inventario automática

## 📋 Requisitos

- Python 3.8+
- Cuenta DMarket con API keys
- Balance en USD en DMarket

## ⚙️ Instalación

1. **Clonar repositorio:**
```bash
git clone <repo-url>
cd cs2
```

2. **Instalar dependencias:**
```bash
pip install -r requirements.txt
```

3. **Configurar variables de entorno:**
Crear archivo `.env`:
```
DMARKET_PUBLIC_KEY=tu_public_key
DMARKET_SECRET_KEY=tu_secret_key
DMARKET_FEE_PERCENTAGE=0.05
DMARKET_MIN_FEE_USD=0.01
```

## 🎮 Uso

**Ejecutar sistema de trading:**
```bash
python trading_real_consola.py
```

### Opciones del menú:
1. 💰 Ver Balance y ROI
2. 📊 Ver KPIs Completos  
3. 🔍 Escanear Oportunidades
4. 🚀 Ejecutar Trade Manual
5. 📦 Ver Portfolio
6. 🤖 Sesión Trading Automático
7. ❌ Salir

## ⚠️ Advertencias

- **DINERO REAL**: Este sistema usa dinero real de tu cuenta DMarket
- **RIESGO**: El trading conlleva riesgo de pérdidas
- **PRUEBAS**: Comienza con cantidades pequeñas
- **SUPERVISIÓN**: Supervisa el bot regularmente

## 📁 Estructura del Proyecto

```
cs2/
├── core/                    # Módulos principales
│   ├── dmarket_connector.py # Conexión API DMarket
│   ├── market_analyzer.py   # Análisis de mercado
│   ├── strategy_engine.py   # Motor de estrategias
│   ├── real_trader.py       # Ejecutor de trades
│   ├── kpi_tracker.py       # Seguimiento KPIs
│   ├── inventory_manager.py # Gestión inventario
│   ├── risk_manager.py      # Gestión de riesgo
│   ├── data_manager.py      # Gestión de datos
│   └── models.py            # Modelos de datos
├── trading_real_consola.py  # Aplicación principal
├── requirements.txt         # Dependencias
├── .env                     # Variables de entorno
└── cs2_trading.db          # Base de datos SQLite
```

## 🛠️ Configuración Avanzada

### Estrategias Disponibles:
- **Basic Flip**: Compra/venta rápida con margen mínimo
- **Snipe**: Detección de precios por debajo del mercado
- **Arbitraje**: Diferencias de precio entre plataformas

### Parámetros Configurables:
- Profit mínimo por trade
- Máximo USD por trade
- Spread máximo permitido
- Liquidez mínima requerida

## 📞 Soporte

Para problemas o preguntas, revisar logs en la consola o verificar:
- Configuración de API keys
- Balance disponible en DMarket
- Conexión a internet
- Estado de la API de DMarket

---
**⚠️ DISCLAIMER**: Este software es para fines educativos. El trading conlleva riesgo financiero.
