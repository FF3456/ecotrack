# EcoTrack - Aplicación Full Stack Optimizada

## Estructura
- `/cliente`: React + Vite + Tailwind CSS + Terser v5 + Compresión Gzip/Brotli + Code Splitting
- `/servidor`: Node.js + Express + Mongoose + Swagger + Compression Middleware + Helmet
- `docker-compose.yml`: Despliegue completo con MongoDB, Backend y Frontend Nginx

## Cambios y Correcciones Incluidos
1. **Solución a Error de Vite v3+**: Inclusión explícita de `terser` (^5.24.0) en `cliente/package.json`.
2. **Estilos con Tailwind CSS**: Integración completa con `tailwind.config.js`, `postcss.config.js` e `index.css`.
3. **MongoDB Cloud (Atlas) & Local**: Soporte dinámico para cadena `MONGO_URI` en entorno local y producción.
4. **Despliegue Desacoplado**: Configuración de `VITE_API_URL` para despliegue independiente en Vercel/Render.

## Ejecución con Docker
```bash
docker-compose up --build
```
- Frontend: http://localhost
- Backend: http://localhost:5000
- Swagger Docs: http://localhost:5000/api-docs
