# TP06 — App de notas con Docker Compose

## Descripción
Aplicación full stack de notas implementada con Docker Compose.

## Arquitectura
- Frontend: Nginx sirviendo HTML y proxy inverso
- Backend: Flask API
- Base de datos: PostgreSQL

## Servicios
- notes-frontend → puerto 80
- notes-backend → API interna
- notes-db → base de datos

## Ejecución

```bash
docker compose up -d --build

Verificación
curl http://localhost/health

Healthcheck
bash scripts/healthcheck.sh

Tecnologías utilizadas
Docker / Docker Compose
Python / Flask
PostgreSQL
Nginx
