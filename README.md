# Asistente para Cirugía de Cataratas (MVP)

Proyecto ejecutable con Next.js + TypeScript + Tailwind + Supabase.

## Requisitos
- Node.js 20+
- npm 10+
- Proyecto Supabase

## Ejecutar local
1. Instala dependencias:
   ```bash
   npm install
   ```
2. Copia variables de entorno:
   ```bash
   cp .env.example .env.local
   ```
3. Completa las claves de Supabase en `.env.local`.
4. Ejecuta:
   ```bash
   npm run dev
   ```
5. Abre [http://localhost:3000](http://localhost:3000).

## Base de datos
1. Ejecuta `supabase/schema.sql`.
2. Ejecuta `supabase/rls.sql`.

## Scripts
- `npm run dev`
- `npm run build`
- `npm run start`
- `npm run lint`
- `npm run typecheck`

## Estructura clave
- `src/app` rutas y UI
- `src/app/actions` server actions
- `src/app/api` endpoints de documentos e IA
- `src/lib/iol` cálculo modular de LIO
- `supabase/` esquema SQL + políticas RLS
- `docs/` arquitectura y deploy

## Reglas clínicas implementadas
- IA solo asistencial/documental; no decisiones clínicas.
- Cálculo de LIO trazable y validable.
- Recetas/indicaciones sujetas a aprobación médica.
