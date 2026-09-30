# Zettro

Sistema de gestión ERP para comercios argentinos — ventas, stock, AFIP, RRHH, tesorería y más.

## Requisitos

- Node.js 22+
- Windows 10/11 (producción)

## Setup

```bash
npm install
```

## Desarrollo

```bash
npm run dev
```

## Build (Windows)

```bash
npm run build:win
```

## Tests

```bash
npm run test:unit        # unitarios
npm run test:ci          # pipeline completo
npm run test:coverage    # con cobertura (umbrales 70/60)
```

## Estructura

- `src/main/` — proceso principal (Electron)
- `src/preload/` — bridge IPC
- `src/renderer/` — interfaz (React)
- `src/shared/` — tipos y constantes compartidos
- `prisma/` — esquema de base de datos
- `resources/` — recursos de runtime (watchdog, iconos)
