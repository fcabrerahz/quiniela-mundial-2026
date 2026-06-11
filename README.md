# ⚽ Quiniela Mundial 2026

App web para llenar la quiniela del Mundial 2026 con marcadores exacto partido por partido.

## Características

- 🗓 **72 partidos** organizados por fecha (11–27 de junio)
- ⌨️ **Marcadores exactos** — ingresa los goles de local y visitante
- 🏆 **Resultado automático** — muestra 1/X/2 calculado al instante
- 💾 **Guarda tu progreso** — usa localStorage, no pierdes nada si cierras el tab
- 📊 **Resumen** — tabla completa con todos tus picks y partidos pendientes
- ⬇️ **Exportar CSV** — descarga tu quiniela en Excel
- 📱 **Responsive** — funciona en móvil y escritorio

## Cómo publicar en GitHub Pages

### Paso 1 — Sube el repositorio a GitHub

```bash
git init
git add .
git commit -m "Quiniela Mundial 2026"
gh repo create quiniela-mundial-2026 --public --source=. --push
```

O manualmente:
1. Crea un repo en [github.com/new](https://github.com/new)
2. Nómbralo `quiniela-mundial-2026`
3. Súbelo con tu cliente de Git o arrastrando los archivos

### Paso 2 — Activa GitHub Pages

1. Ve a tu repo → **Settings** → **Pages**
2. En *Source*, selecciona **Deploy from a branch**
3. Rama: `main`, carpeta: `/ (root)`
4. Clic en **Save**

### Paso 3 — Comparte el link

En ~1 minuto tu app estará disponible en:

```
https://TU-USUARIO.github.io/quiniela-mundial-2026/
```

Comparte ese link con todos los participantes. Cada quien llena su propia quiniela en su dispositivo y puede exportar el CSV para enviártelo.

## Estructura del proyecto

```
quiniela-mundial-2026/
└── index.html    ← toda la app en un solo archivo
└── README.md
```

## Uso

1. Escribe tu nombre y la fecha de entrega arriba
2. Ingresa el marcador de cada partido (goles local : goles visitante)
3. El resultado 1/X/2 aparece automáticamente en verde
4. Usa **Ver resumen** para revisar todo antes de entregar
5. Usa **Exportar CSV** para descargar tu quiniela

## Puntuación (sugerida)

Puedes usar el CSV exportado para calcular puntos. Sugerencias:

| Acierto | Puntos |
|---------|--------|
| Marcador exacto | 3 pts |
| Solo el resultado correcto (1/X/2) | 1 pt |
| Incorrecto | 0 pts |
