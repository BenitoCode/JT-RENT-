# Ficha — JT Rent (web de cliente)

## Proyecto
- Nombre: JT Rent — alquiler de scooters en Málaga. Cliente de Benitek.
- Repo: BenitoCode/JT-RENT- (único válido; los repos jt-rent y jt_rent son antiguos: no usarlos).
- Tipo: web de cliente · landing · Skills: web-base
- Objetivo: conseguir consultas de alquiler por WhatsApp. Bilingüe ES/EN.
- Dominio: https://jt-rent.com

## Tecnologías
- Next.js 16 (App Router, `output: "export"`), React 19, TypeScript, Tailwind CSS 4, Lucide.
- La web vive en `jtrent/`; la raíz solo define los workspaces para Hostinger.
- Tests: lógica (node test) y navegador (Playwright).
- Despliegue: Hostinger estático (build → `jtrent/out`), Node 24. Detalles en DEPLOY_HOSTINGER.md.

## Comandos (desde `jtrent/`)
- `npm run dev` → http://127.0.0.1:3000/es/
- `npm run build` · `npm run typecheck` · `npm run lint` · `npm test` · `npm run test:e2e`

## Reglas de este proyecto
- Es web de cliente: prioriza estabilidad y no cambies precios, condiciones ni textos comerciales sin mi indicación.
- Antes de escribir código Next.js, sigue `jtrent/AGENTS.md` (esta versión tiene cambios incompatibles).
- Antes de cambiar diseño o contenido, lee `jtrent/README.md` y `jtrent/DESIGN_DECISIONS.md`.
- Trabaja sección por sección y espera mi aprobación antes de continuar.
- Registra cada decisión de diseño aprobada en `DESIGN_DECISIONS.md`.
- Textos en `es.json` y `en.json`, siempre con las mismas claves.
- Precios solo en `src/data/motorcycles.ts`. No inventes motos, fotos, reseñas ni datos de contacto.
- No incorpores la fuente Helvetica Neue hasta confirmar su licencia web.
- Web estática: nada de API routes ni funciones de servidor.
- Variables en `.env.local`; nunca lo subas a Git.
- Ejecuta typecheck, lint y test antes de cada commit.

## Estado
- Publicada en https://jt-rent.com (Hostinger).
- Último cambio: 26 oct 2026 (reseña de Google).
- Cada push a `main` se publica automáticamente: no hagas push sin mi permiso.

## Decisiones aprobadas
- Ver `jtrent/DESIGN_DECISIONS.md` (fuente única).

## Tareas pendientes
- Ver "Pendiente de recursos o información" en `DESIGN_DECISIONS.md`.

## Próximo paso
- Por definir.
