# 🧩 Cómo enviar un JSON en Postman

## 1️⃣ Crear la petición
- Abre **Postman**.
- Haz clic en **New** → **Request** o en el botón +.
- Escribe la **URL del endpoint** (por ejemplo: ```https://api.miapp.com/usuarios```).

## 2️⃣ Elegir el método
En el menú desplegable a la izquierda de la URL selecciona:
- ```POST``` si vas a crear un recurso.
- ```PUT``` si vas a actualizar.
- ```PATCH``` si vas a modificar parcialmente.

## 3️⃣ Escribir el cuerpo (Body)
1. Ve a la pestaña **Body**.
2. Marca **raw**.
3. En el menú de la derecha, selecciona **JSON**.
4. Escribe tu contenido, por ejemplo:
```json
{
  "nombre": "Néstor",
  "correo": "nestor@example.com",
  "activo": true
}
```

## 4️⃣ Revisar los encabezados
Asegúrate de tener este encabezado:
```pgsql
Content-Type: application/json
```
> Postman normalmente lo agrega solo.

## 5️⃣ Enviar y revisar la respuesta
- Haz clic en **Send**.
- Abajo verás:
  - El **código de estado** (```200 OK```, ```201 Created```, etc.)
  - El **Body** de la respuesta (también en JSON, si aplica).
