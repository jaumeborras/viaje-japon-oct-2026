# Viaje a Japón · Jaime + Marina · Octubre 2026

Este archivo contiene el contexto completo del proyecto para retomar la planificación.

---

## Datos base

- **Viajeros:** Jaime y Marina (pareja)
- **Vuelo llegada:** 3 oct 2026, 9:30 en Narita (NRT)
- **Vuelo salida:** 17 oct 2026, 11:10 desde Narita (NRT)
- **Duración:** 14 noches en Japón
- **Idioma de comunicación:** español
- **Moneda:** SIEMPRE en euros (€). Nunca yen ni otras divisas.

## Reglas de trabajo

- **NO INVENTAR nada.** Si no lo sabes, dilo. Aplica a nombres, precios exactos, disponibilidad, direcciones específicas, horarios, restaurantes concretos.
- Precios y horarios pueden haber cambiado; siempre presentarlos como orientativos.
- Preferencia por respuestas **concisas y directas**, sin sobre-explicar. Ir paso por paso, no arrollar con opciones.
- El usuario prefiere pocas opciones bien elegidas frente a listas largas.
- Cuando haga falta buscar información concreta (hoteles, horarios, precios), usar web search.

## Filosofía de alojamiento

Priorizan **experiencias culturales tradicionales** por encima de hoteles estándar:
- Ryokan tradicional donde tenga sentido (Kawaguchiko, Takayama)
- Shukubo (monasterio) en Koyasan — reserva más urgente
- Kioto: se optó finalmente por hotel estándar (Agora Kyoto Karasuma) en vez de machiya
- Hoteles funcionales en ciudades donde el alojamiento aporta poco culturalmente (Tokio, Osaka)

**Presupuesto orientativo:** 90-150 €/noche para dos, con flexibilidad para estirar hasta 200-250 € en experiencias especialmente significativas (ryokan con onsen + kaiseki, shukubo).

---

## Itinerario actual (14 noches, 6 paradas)

| # | Fechas | Noches | Base | Estado alojamiento |
|---|---|---|---|---|
| 1 | 3–5 oct | 2 | Tokio (Shinjuku) | ✅ Hotel Kabuki reservado |
| 2 | 5–6 oct | 1 | Kawaguchiko | ✅ Tsunagaru Camp Resort QOONEL+ reservado |
| 3 | 6–10 oct | 4 | Kioto | ✅ Agora Kyoto Karasuma reservado · 1 día a Nara |
| 4 | 10–11 oct | 1 | Koyasan | Pendiente (shukubo) ⚠️ URGENTE |
| 5 | 11–15 oct | 4 | Kanazawa | Pendiente · base para Takayama + Shirakawa-go |
| 6 | 15–17 oct | 2 | Tokio (Asakusa/Ueno) | Pendiente |

**Cambio de estructura (julio 2026):** Takayama deja de ser parada con noche y pasa a excursión de día desde Kanazawa (junto con Shirakawa-go). Osaka pierde la noche (se ve de paso entre Koyasan y Kanazawa). Kioto pasa a 4 noches (incluye día a Nara). Tokio pasa a 4 noches repartidas 2+2. Kanazawa → Tokio ahora es shinkansen Hokuriku directo (~2h30).

**Excursiones de día PLANIFICADAS (ya dentro del itinerario, sin noche):**
- **Nara** — uno de los 4 días de Kioto (~45 min en tren).
- **Takayama** — desde Kanazawa (bus Nohi ~2h15 por trayecto).
- **Shirakawa-go** — desde Kanazawa (bus ~1h15).

**Excursiones de día OPCIONALES (posibilidades, no decididas):**
- **Kobe** — desde la zona de Osaka (~20-30 min).
- **Kamakura** — desde Tokio (~1h). Cabe en cualquiera de los dos bloques de Tokio.
- **Miyajima** — isla junto a Hiroshima (oeste). ~2h por trayecto; la más exigente, mejor como noche propia si se hace.
- **Osaka** — ya no tiene noche; se ve de paso (comida/Dotonbori) entre Koyasan y Kanazawa.

**Nota importante sobre Kioto:** ahora 4 noches (~3 días completos + partes), uno de ellos dedicado a Nara. Sigue habiendo más contenido del que cabe: priorizar en su momento.

---

## Transiciones entre paradas

| Trayecto | Medio | Tiempo aprox. |
|---|---|---|
| Tokio → Kawaguchiko | Bus Fujikyu desde Shinjuku | 1h45 |
| Kawaguchiko → Kioto | Bus a Mishima + shinkansen | ~3h30 |
| Kioto → Koyasan | Kioto → Namba + Nankai Koya + funicular | ~2h45 |
| Koyasan → Kanazawa | Baja a Osaka (de paso) + Thunderbird/shinkansen vía Tsuruga | ~5h |
| Kanazawa → Tokio | Hokuriku Shinkansen directo | ~2h30 |

**Excursiones de día desde Kanazawa:**
| Kanazawa → Takayama | Bus Nohi | 2h15 |
| Kanazawa → Shirakawa-go | Bus Nohi/Hokutetsu | ~1h15 |

---

## Prioridades de reserva (por orden)

1. **Shukubo en Koyasan** (10 oct) — pocas plazas, meses de antelación
2. **Alojamiento en Kanazawa** (11-15 oct, 4 noches) — base para Takayama y Shirakawa; opción ryokan tradicional
3. Hotel última noche(s) en Tokio (15-17 oct) — puede esperar

---

## Puntos de interés por ciudad

Ver `pois.md` para la lista completa por ciudad.

**Aviso al Claude Code:** los puntos son *posibilidades* que Jaime ha ido guardando, NO son un itinerario cerrado. No planificar como si todo se fuera a visitar.

---

## Estado del mapa interactivo

Mapa standalone en `ruta_japon.html` (ver el archivo para el estado actual de marcadores/paneles).

**Cuando cambies el itinerario:** actualiza el array `stops` en el `<script>` del HTML. La estructura de cada parada es:

```js
{
  n: número, name: "...", dates: "X → Y oct", nights: N,
  lat: X, lng: Y,
  notes: "...",
  todo: ["...", "..."],
  hotel: "...", booked: true|false,
  bookingUrl: "..." // opcional
}
```

---

## Historial de decisiones

- **Hakone descartado** por presupuesto (ryokan con kaiseki excedía rango). Sustituido por Kawaguchiko.
- **Reorganización (jul 2026):** Kanazawa pasa a ser base de 4 noches para Takayama y Shirakawa-go como excursiones de día. Takayama deja de tener noche propia. Osaka pierde la noche (de paso). Kioto sube a 4 noches (con día a Nara). Tokio sube a 4 noches (2+2).
- **Shirakawa-go se hace como excursión de día desde Kanazawa** (antes desde Takayama).
- **Ruta Kanazawa → Tokio:** shinkansen Hokuriku directo (~2h30), sustituye al antiguo Wide View Hida.
- **Nombre del usuario:** Jaime (Marina es la pareja). No inventar apellidos ni otros datos.

---

## Cosas pendientes concretas

1. Cerrar shukubo Koyasan (urgente)
2. Cerrar alojamiento en Kanazawa (4 noches, base de la zona)
3. Definir contenido de POIs para Kanazawa y Takayama (Jaime irá pasando imágenes)
4. Cuando toque: reservas de trenes y buses (Fujikyu, shinkansen Mishima-Kioto, Nankai Koya, Thunderbird+Hokuriku, Hokuriku Kanazawa-Tokio, buses Nohi a Takayama/Shirakawa)
5. Verificar si compensa algún pase regional (Hokuriku Arch Pass encaja bien: Tokio–Kanazawa–Osaka; valorar también Kansai para Koyasan/Nara)

---

## Preferencias específicas del HTML

- Fuentes: Fraunces (serif) + Inter (sans) + JetBrains Mono (mono)
- Paleta: papel washi (#F1E9D6), tinta (#1B1F2A), persimmon (#C84A28), musgo (#5E6B3D)
- Panel a pantalla completa (no popup pequeño)
- Popup NO permanente: se cierra ~220ms después de salir del marcador
