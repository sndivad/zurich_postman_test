# Postman Collections

Este proyecto incluye colecciones de Postman diseñadas para probar y verificar dos tipos de endpoints: un endpoint GET y un endpoint POST.

## Requisitos

Para ejecutar estas colecciones, necesitas:

- [Postman](https://www.postman.com/downloads/) instalado en tu máquina.
- Acceso a los endpoints que deseas probar.

## Endpoints Incluidos

### Endpoint GET

#### Verificaciones:
1. **Código de respuesta:** La respuesta del endpoint debe ser un código HTTP `200 OK`.
2. **Estructura de la respuesta:** La respuesta debe ser un array.

#### Ejemplo de Uso:
- URL del endpoint: `https://680537f4ca467c15be68936d.mockapi.io/users/users`
- Ejecuta la solicitud en Postman y verifica que:
  - El código de respuesta sea `200`.
  - La respuesta sea un array válido.

![Mi imagen desde Imgur](https://i.imgur.com/yHPyMyX.png)

### Endpoint POST

#### Verificaciones:
1. **Código de respuesta:** La respuesta del endpoint debe ser un código HTTP `201 Created`.
2. **Contenido de la respuesta:** La respuesta debe incluir el campo `name` y `nombre introducido`.
3. **Tipo de dato:** El campo `testingvalue` debe ser de tipo booleano.

#### Ejemplo de Uso:
- URL del endpoint: `https://680537f4ca467c15be68936d.mockapi.io/users/users`
- Cuerpo del ejemplo para la solicitud:


  ```json
  {
    "nombre": "Ejemplo",
    "testingvalue": true
  }

![Mi imagen desde Imgur](https://i.imgur.com/8WeCpik.png)


### Verificación de la Solicitud

Ejecuta la solicitud en Postman y verifica que:
- El código de respuesta sea `201`.
- La respuesta incluya un campo `nombre`.
- El campo `testingvalue` sea de tipo booleano.

### Cómo Importar la Colección

1. Abre Postman.
2. Haz clic en **Importar**.
3. Selecciona el archivo de colección (.json) proporcionado.
4. Ejecuta las solicitudes y verifica los resultados descritos.


