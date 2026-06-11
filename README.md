# ⚽ Quiniela Mundial 2026

App web completa para pronosticar el Mundial 2026 — fase de grupos, rondas eliminatorias, tabla de posiciones automática y sistema de puntos en tiempo real.

## 🌐 Cómo usarla

| Archivo | Quién la usa | Para qué |
|---|---|---|
| `index.html` | Jugadores | Llenar marcadores de los 72 partidos de grupos |
| `bracket.html` | Jugadores | Pronosticar R32, Octavos, Cuartos, Semis y Final |
| `admin.html` | Solo el organizador | Ingresar resultados reales y ver la tabla de posiciones |

### Flujo del jugador
1. Abre `index.html` → escribe tu nombre → llena los marcadores de los 72 partidos
2. Haz clic en **🏆 Bracket** → llena tus pronósticos para las rondas eliminatorias
3. Clic en **⬇ Exportar quiniela completa** → manda el CSV al organizador

### Flujo del organizador
1. Abre `admin.html` → ingresa la contraseña
2. Conforme se juegan los partidos, ingresa los resultados reales (por ronda)
3. Importa los CSV de los jugadores arrastrándolos a la zona de carga
4. La tabla de posiciones se actualiza en tiempo real automáticamente

---

## ⭐ Sistema de puntuación

| Ronda | Marcador exacto | Solo ganador correcto |
|---|---|---|
| Fase de Grupos (72 partidos) | **3 pts** | **1 pt** |
| R32 · Octavos · Cuartos · Semis | **5 pts** | **2 pts** |
| Final | **10 pts** | **3 pts** |

---

## 🏆 Bracket — 100% FIFA oficial

El bracket implementa las **495 combinaciones oficiales** del Anexo C del reglamento de FIFA. Una vez conocidos los 8 mejores terceros de la fase de grupos, el sistema determina automáticamente qué equipo se enfrenta a quién en la Ronda de 32, sin duplicados ni errores.

Los cruces fijos de la Ronda de 32:

| Partido | Local | Visitante |
|---|---|---|
| M73 | 2° Grupo A | 2° Grupo B |
| M74 | 1° Grupo E | Mejor 3° (A/B/C/D/F) |
| M75 | 1° Grupo F | 2° Grupo C |
| M76 | 1° Grupo C | 2° Grupo F |
| M77 | 1° Grupo I | Mejor 3° (C/D/F/G/H) |
| M78 | 2° Grupo E | 2° Grupo I |
| M79 | 1° Grupo A | Mejor 3° (C/E/F/H/I) |
| M80 | 1° Grupo L | Mejor 3° (E/H/I/J/K) |
| M81 | 1° Grupo D | Mejor 3° (B/E/F/I/J) |
| M82 | 1° Grupo G | Mejor 3° (A/E/H/I/J) |
| M83 | 2° Grupo K | 2° Grupo L |
| M84 | 1° Grupo H | 2° Grupo J |
| M85 | 1° Grupo B | Mejor 3° (E/F/G/I/J) |
| M86 | 1° Grupo J | 2° Grupo H |
| M87 | 1° Grupo K | Mejor 3° (D/E/I/J/L) |
| M88 | 2° Grupo D | 2° Grupo G |

---

## 🔒 Seguridad del admin

`admin.html` está protegida por contraseña. Para cambiarla, busca esta línea en el archivo y edítala:

```js
const ADMIN_PASSWORD = 'mundial2026';
```

Solo comparte `index.html` y `bracket.html` con los participantes. Guarda la URL de `admin.html` para ti.

---

## 🚀 Publicar en GitHub Pages

### Paso 1 — Sube los archivos
1. Crea un repo en [github.com/new](https://github.com/new) → nombre `quiniela-mundial-2026` → **Public**
2. Sube los 4 archivos: `index.html`, `bracket.html`, `admin.html`, `README.md`

### Paso 2 — Activa GitHub Pages
Settings → Pages → Source: **Deploy from a branch** → rama `main`, carpeta `/ (root)` → **Save**

### Paso 3 — Comparte
En ~1 minuto tu app estará en:
```
https://TU-USUARIO.github.io/quiniela-mundial-2026/
```

---

## 📋 Características

- ✅ 72 partidos de grupos con fecha, equipos y sede
- ✅ Clasificación automática de grupos (puntos, diferencia de goles, goles a favor)
- ✅ 8 mejores terceros calculados automáticamente
- ✅ Bracket R32 → Octavos → Cuartos → Semis → Final generado desde tus picks
- ✅ 495 combinaciones oficiales de FIFA para asignación de terceros
- ✅ CSV combinado (grupos + eliminatorias) para importar en admin
- ✅ Tabla de posiciones en tiempo real conforme entran resultados
- ✅ Detalle partido a partido por jugador (clic en su nombre)
- ✅ Exportar tabla de posiciones en CSV
- ✅ Guarda automáticamente en el navegador (localStorage)
- ✅ Contraseña de admin
- ✅ Responsive — funciona en móvil y escritorio

## 📅 Calendario del torneo

- **Fase de grupos:** 11 – 27 de junio de 2026
- **Ronda de 32:** 28 jun – 3 jul
- **Octavos de final:** 4 – 7 jul
- **Cuartos de final:** 9 – 11 jul
- **Semifinales:** 14 – 15 jul
- **Final:** 19 de julio de 2026 · MetLife Stadium, Nueva York/NJ
