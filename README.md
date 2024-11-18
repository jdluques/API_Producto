# API_Producto

## POST: Crear Producto
```json
{
  "productoID": "P12345",
  "nombre": "Producto de Ejemplo",
  "descripcion": "Descripción detallada del producto.",
  "precio": 100.00,
  "stock": 50
}
```
## GET: Consultar Producto
```
Query Params (solo uno es necesario, tenantID o productoID):
tenantID: "202411-123e4567-e89b-12d3-a456-426614174000"
productoID: "P12345"
```
## PUT: Actualizar Producto
```json
{
  "productoID": "P12345",
  "tenantID": "202411-123e4567-e89b-12d3-a456-426614174000",
  "nombre": "Producto Actualizado",
  "descripcion": "Nueva descripción",
  "precio": 120.00,
  "stock": 40
}
```
## DELETE: Eliminar Producto
```json
{
  "productoID": "P12345",
  "tenantID": "202411-123e4567-e89b-12d3-a456-426614174000"
}
```
## GET: Listar Productos
```
Query Params (opcional para paginación):
limit: "10" (cantidad máxima de productos por página)
lastEvaluatedKey: "{\"productoID\": \"P12345\", \"tenantID\": \"202411-123e4567-e89b-12d3-a456-426614174000\"}" (para continuar desde el último producto evaluado)

```

## ENDPOINTS:
```
  POST - https://dcd20ifa4b.execute-api.us-east-1.amazonaws.com/dev/productos/create
  GET - https://dcd20ifa4b.execute-api.us-east-1.amazonaws.com/dev/productos/get
  PUT - https://dcd20ifa4b.execute-api.us-east-1.amazonaws.com/dev/productos/update
  DELETE - https://dcd20ifa4b.execute-api.us-east-1.amazonaws.com/dev/productos/delete
  GET - https://dcd20ifa4b.execute-api.us-east-1.amazonaws.com/dev/productos/list
```
