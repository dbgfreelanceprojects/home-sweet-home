# Endpoints iniciales del API REST

## Autenticación
- POST `/api/auth/register`    → Crear usuario
- POST `/api/auth/login`       → Iniciar sesión

## Hogares
- GET `/api/homes`             → Listar hogares del usuario actual
- POST `/api/homes`            → Nuevo hogar
- GET `/api/homes/{id}`        → Ver hogar

## Gastos
- GET `/api/expenses?homeId=`  → Listar gastos de un hogar
- POST `/api/expenses`         → Nuevo gasto

## Almacén (Productos)
- GET `/api/products?homeId=`  → Productos en almacén
- POST `/api/products`         → Añadir producto

## Compras
- GET `/api/purchases?homeId=` → Lista de compras realizadas
- POST `/api/purchases`        → Nueva compra

## Notas técnicas

Todas las rutas protegidas requieren autenticación JWT (enviar token como header `Authorization`).
