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
- Machiya (casa tradicional) en Kioto
- Hoteles funcionales en ciudades donde el alojamiento aporta poco culturalmente (Tokio, Osaka)

**Presupuesto orientativo:** 90-150 €/noche para dos, con flexibilidad para estirar hasta 200-250 € en experiencias especialmente significativas (ryokan con onsen + kaiseki, shukubo).

---

## Itinerario actual (14 noches, 8 paradas)

| # | Fechas | Noches | Base | Estado alojamiento |
|---|---|---|---|---|
| 1 | 3–5 oct | 2 | Tokio (Shinjuku) | 🔶 Via Inn Shinjuku decidido, sin reservar ~210 € |
| 2 | 5–6 oct | 1 | Kawaguchiko | Pendiente |
| 3 | 6–8 oct | 2 | Kioto | Pendiente (machiya) |
| 4 | 8–10 oct | 2 | Osaka | Pendiente |
| 5 | 10–11 oct | 1 | Koyasan | Pendiente (shukubo) ⚠️ URGENTE |
| 6 | 11–13 oct | 2 | Kanazawa | Pendiente |
| 7 | 13–16 oct | 3 | Takayama | Pendiente (con día completo a Shirakawa-go) |
| 8 | 16–17 oct | 1 | Tokio (Asakusa/Ueno) | Pendiente |

**Excursiones de día opcionales (no reservadas, posibilidades):**
- **Nara** — desde Kioto u Osaka (~40-45 min).
- **Kobe** — desde Osaka (~20-30 min), cabría como medio día en el bloque de Osaka.
- **Kamakura** — desde Tokio (~1h). Solo encaja desde Tokio, que va justo; pendiente de decidir cómo hacer hueco.
- **Miyajima** — isla junto a Hiroshima (oeste). ~2h por trayecto desde Osaka; la más exigente como día suelto, valorar como noche propia.

Ninguna añade noche. Se dejan como marcadores opcionales en el mapa por si se reorganiza el itinerario.

**Nota importante sobre Kioto:** con 2 noches solo hay ~1 día completo real. El usuario tiene contenido para 3 días recopilado, pero prefiere dejarlo como "posibilidades" y decidir prioridades más adelante.

---

## Transiciones entre paradas

| Trayecto | Medio | Tiempo aprox. |
|---|---|---|
| Tokio → Kawaguchiko | Bus Fujikyu desde Shinjuku | 1h45 |
| Kawaguchiko → Kioto | Bus + shinkansen vía Mishima | ~3h30 |
| Kioto → Osaka | Shinkansen o JR/Hankyu | 15-45 min |
| Osaka → Koyasan | Nankai Koya Line + funicular | ~2h |
| Koyasan → Kanazawa | Funicular + tren + Thunderbird vía Osaka | ~5h |
| Kanazawa → Takayama | Bus Nohi | 2h15 |
| Takayama → Tokio | Wide View Hida + shinkansen | ~4h |

---

## Prioridades de reserva (por orden)

1. **Shukubo en Koyasan** (11 oct) — pocas plazas, meses de antelación
2. **Ryokan / minshuku en Kawaguchiko** (5 oct) — vistas al Fuji
3. **Ryokan en Takayama** (13-16 oct) — con opción de temple stay (Zenkoji)
4. **Machiya en Kioto** (6-8 oct)
5. Hoteles en Osaka, Kanazawa y última noche en Tokio — pueden esperar

---

## Puntos de interés por ciudad

Ver `pois.md` para la lista completa por ciudad.

**Aviso al Claude Code:** los puntos son *posibilidades* que Jaime ha ido guardando, NO son un itinerario cerrado. No planificar como si todo se fuera a visitar.

---

## Estado del mapa interactivo

Se ha construido un HTML standalone (`ruta_japon.html`) con:
- Mapa Leaflet centrado en Japón (tiles CartoDB Positron)
- 8 marcadores numerados con la ruta
- Nara como marcador opcional (círculo hueco, borde discontinuo)
- Panel a pantalla completa al hacer hover en cualquier parada, con lista completa de POIs
- Botón "Ver reserva" en paradas con `bookingUrl` configurada
- Barra lateral con timeline del itinerario

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
- **Kioto reducido de 3 a 2 noches** para poder añadir 1 noche a Takayama (3 en total, con día completo a Shirakawa-go).
- **Shirakawa-go se hace como excursión de día desde Takayama**, no como noche independiente.
- **Nombre del usuario:** Jaime (Marina es la pareja). No inventar apellidos ni otros datos.

---

## Cosas pendientes concretas

1. Cerrar alojamiento en Kawaguchiko (siguiente conversación)
2. Cerrar shukubo Koyasan (urgente)
3. Definir contenido de POIs para Osaka, Kanazawa, Takayama (Jaime irá pasando imágenes)
4. Cuando toque: reservas de shinkansen y buses (Wide View Hida, Nohi, Fujikyu, Romancecar N/A)
5. Verificar si compensa algún pase regional (Hokuriku Arch Pass podría encajar)

---

## Preferencias específicas del HTML

- Fuentes: Fraunces (serif) + Inter (sans) + JetBrains Mono (mono)
- Paleta: papel washi (#F1E9D6), tinta (#1B1F2A), persimmon (#C84A28), musgo (#5E6B3D)
- Panel a pantalla completa (no popup pequeño)
- Popup NO permanente: se cierra ~220ms después de salir del marcador
