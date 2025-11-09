# 🌍 Cómo usar variables de entorno en Postman
## 1️⃣ ¿Qué son?
Las **variables de entorno** te permiten **guardar valores reutilizables**, como URLs, tokens o IDs, para no tener que escribirlos en cada petición.

Por ejemplo, puedes tener una variable ```{{base_url}}``` en lugar de repetir ```https://api.miapp.com``` en todas tus peticiones.

## 2️⃣ Crear un entorno
1. En la esquina superior derecha, haz clic en el icono del **ojo 👁️ (Environment)**.
2. Elige “**Add**” o “**Manage Environments**”.
3. Asigna un nombre, por ejemplo: **Desarrollo**.
4. Agrega tus variables, por ejemplo:
- ```base_url``` → ```https://api.dev.miapp.com```
- ```token``` → ```abc123xyz```
5. Guarda los cambios.

## 3️⃣ Usarlas en tus peticiones
En lugar de escribir la URL completa, usa llaves dobles:
```bash
{{base_url}}/usuarios
```
Y en los encabezados puedes usar:
```css
Authorization: Bearer {{token}}
```

## 4️⃣ Cambiar de entorno fácilmente
- En la parte superior derecha, selecciona el entorno que quieras usar (por ejemplo, Producción o Desarrollo).
- Postman reemplazará automáticamente las variables por sus valores del entorno activo.

## 5️⃣ Extra: variables globales o de colección
- **Globales**: disponibles en todo Postman.
- **De colección**: solo dentro de una colección específica.
Usa el tipo según tu necesidad para mantener tu trabajo ordenado.
