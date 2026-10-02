<div align="center">

# 🗑️ EcoRuta

### Le enseñamos a los camiones de basura a pensar

[![Status](https://img.shields.io/badge/status-MVP%20funcional-3ddc97?style=for-the-badge)]()
[![Ahorro](https://img.shields.io/badge/ahorro%20estimado-32%25%20combustible-FFB703?style=for-the-badge)]()
[![IA](https://img.shields.io/badge/motor-optimizaci%C3%B3n%20de%20rutas-6A4C93?style=for-the-badge)]()
[![Mercado](https://img.shields.io/badge/mercado-municipios%20%2B%20campus-FF6B6B?style=for-the-badge)]()

**Rutas de recolección que se adaptan cada día a cuánta basura hay realmente — no a un mapa fijo de hace 10 años.**

</div>

---

## 🤔 El problema que nadie mira

Cada camión de basura en una ciudad promedio recorre **la misma ruta todos los días**, sin importar si los contenedores están llenos, vacíos o a la mitad. Eso significa:

- Combustible quemado visitando contenedores vacíos.
- Horas extra de personal en rutas más largas de lo necesario.
- Contenedores que se desbordan porque nadie sabía que ya estaban llenos.

Nadie lo optimiza porque nadie lo mide. **Nosotros sí.**

## ⚡ La solución

EcoRuta coloca sensores de bajo costo en los contenedores (nivel de llenado + ubicación) y cada madrugada recalcula, con un algoritmo de optimización de rutas, el recorrido más corto que **solo visita lo que realmente necesita recolección**.

```
Sensores ──► Datos de llenado en tiempo real
     │
     ▼
Motor de optimización ──► Ruta más corta y eficiente
     │
     ▼
App del conductor ──► Navegación + checklist del día
```

## 📊 El número que importa

| Métrica | Ruta fija tradicional | Con EcoRuta |
|---|---|---|
| Kilómetros recorridos / día | 180 km | ~122 km |
| Contenedores visitados sin necesidad | ~40% | ~3% |
| Combustible mensual estimado | $4,200 USD | $2,850 USD |
| Desbordes reportados / mes | 15 | 2 |

*(Datos de piloto simulado con 3 rutas de un municipio de tamaño medio.)*

## 🧩 Cómo está construido

| Componente | Función |
|---|---|
| `sensor-gateway/` | Recibe las lecturas de llenado de cada contenedor |
| `route-engine/` | Calcula la ruta óptima diaria (algoritmo tipo "vehicle routing problem") |
| `driver-app/` | App móvil con el recorrido del día para el conductor |
| `dashboard/` | Panel para el municipio: ahorro, rutas, alertas de contenedores llenos |

Todo corre en contenedores Docker independientes, versionado en Git, para que cada ciudad pueda desplegar su propia instancia sin fricción.

## 🌍 ¿Por qué ahora?

- Las ciudades están bajo presión real de reducir emisiones y costos operativos.
- El hardware de sensores IoT ya es barato — lo que falta es el software que lo aproveche.
- Los campus universitarios y zonas industriales son un mercado de entrada perfecto: control total del terreno, decisiones rápidas, impacto medible en semanas.

## 📈 El plan con tu inversión

1. **Fase piloto** — instrumentar 50 contenedores en un municipio aliado, validar el ahorro real.
2. **Escalar el motor** — pasar de rutas fijas por zona a optimización multi-ciudad.
3. **Vender el dashboard** — el verdadero negocio no es el camión, es el dato: cada municipio paga una suscripción para ver su ahorro en tiempo real.

## 🛠️ Stack

`Python` · `Docker` · `Algoritmos de optimización de rutas` · `Git / GitHub` · `Sensores IoT`

---

<div align="center">

### No vendemos basura. Vendemos los kilómetros que ya no vas a recorrer.

**¿Hablamos de los próximos $10M?**

</div>
