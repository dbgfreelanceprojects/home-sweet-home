# Modelo de Datos

## Entidades principales

### Usuario
- id: long
- email: string
- password: string (hashed)
- nombre: string

### Hogar
- id: long
- nombre: string
- usuarioId: long

### Gasto
- id: long
- descripcion: string
- importe: decimal
- fecha: date
- tipo: string (luz, agua, etc)
- hogarId: long

### Producto (Almacén)
- id: long
- nombre: string
- cantidad: int
- hogarId: long

### Compra
- id: long
- productoId: long
- fecha: date
- cantidad: int
- precio: decimal
- hogarId: long

## Diagrama entidad-relación

*(Puedes añadir aquí un diagrama visual generado en dbdiagram.io, Lucidchart o con texto, y actualizar este archivo conforme evolucione el modelo)*
