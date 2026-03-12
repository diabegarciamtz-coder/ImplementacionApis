# 🚀 Simple Flask API

Pequeña **API REST** desarrollada con **Python** utilizando el framework **Flask** para practicar la creación de endpoints y probar peticiones HTTP con **Postman**.

---

## 📌 Descripción

Este proyecto implementa una API básica que permite realizar operaciones simples sobre usuarios.  
Fue desarrollado como práctica para comprender el funcionamiento de una **API REST**, el manejo de **peticiones HTTP** y el intercambio de datos en **formato JSON**.

La API permite:

- 🔎 Obtener información de un usuario por su **ID**
- ➕ Crear un usuario enviando datos en **JSON**
- 🧪 Probar endpoints mediante herramientas de testing de APIs

---

## 🛠 Tecnologías utilizadas

- **Python 3**
- **Flask**
- **Postman**
- **JSON**

---

## 📂 Estructura del proyecto

```
implementacionapi
│
├── main.py          # Archivo principal donde se define la API
├── README.md        # Documentación del proyecto
└── venv/            # Entorno virtual (no se sube al repositorio)
```

---

## 🖼 Ejemplo de respuestas de la API

### GET /users/<id>

<img width="1918" height="1079" alt="image" src="https://github.com/user-attachments/assets/4795d281-e362-401a-beed-f863b1c22fcb" />

### POST /users

<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/a3b568d7-275e-4a41-9d21-16fc68ba2963" />

### Respuesta en Postman

<img width="1919" height="1078" alt="image" src="https://github.com/user-attachments/assets/c5cc41da-6ed6-4981-9be2-dc1fef56dc15" />

---

# ▶️ Cómo ejecutar el proyecto

## 1️⃣ Clonar el repositorio

```bash
git clone https://github.com/TU_USUARIO/TU_REPOSITORIO.git
```

---

## 2️⃣ Entrar a la carpeta del proyecto

```bash
cd implementacionapi
```

---

## 3️⃣ Crear un entorno virtual

```bash
python -m venv venv
```

---

## 4️⃣ Activar el entorno virtual

### Windows (PowerShell)

```bash
.\venv\Scripts\Activate.ps1
```

### Linux / Mac

```bash
source venv/bin/activate
```

---

## 5️⃣ Instalar dependencias

```bash
pip install flask
```

---

## 6️⃣ Ejecutar la aplicación

```bash
python main.py
```

La API se ejecutará en:

```
http://127.0.0.1:5000
```

---

# 🔗 Endpoints disponibles

## 📥 GET /users/<user_id>

Obtiene la información de un usuario mediante su **ID**.

### Ejemplo de petición

```
GET http://127.0.0.1:5000/users/20
```

### Respuesta

```json
{
  "id": "20",
  "name": "test",
  "telefono": "999-666-333"
}
```

### Query parameters opcionales

También es posible enviar parámetros en la URL:

```
GET /users/20?query=test
```

---

## 📤 POST /users

Permite **crear un nuevo usuario** enviando datos en formato **JSON**.

### Ejemplo de petición

```
POST http://127.0.0.1:5000/users
```

### Body (JSON)

```json
{
  "id": "20",
  "name": "Diana",
  "telefono": "418-107-3293"
}
```

### Respuesta

```json
{
  "id": "20",
  "name": "Diana",
  "telefono": "418-107-3293",
  "status": "user created"
}
```

---

# 🧪 Pruebas

Los endpoints fueron probados utilizando **Postman**, enviando peticiones HTTP de tipo:

- **GET** → para obtener información
- **POST** → para crear nuevos usuarios

Esto permitió verificar que la API responde correctamente y que los datos se procesan adecuadamente.

---

# 📚 Aprendizaje del ejercicio

Este proyecto tuvo como objetivo comprender los **fundamentos de las APIs REST** utilizando **Python y Flask**.

Durante el desarrollo se practicó:

- Definición de **rutas (endpoints)**
- Uso de **métodos HTTP**
- Manejo de **query parameters**
- Recepción de datos en **JSON**
- Envío de respuestas desde el servidor en formato **JSON**
- Pruebas de endpoints utilizando **Postman**

---

# 📄 Licencia

Este proyecto fue desarrollado **con fines educativos y de práctica**.

**Autora:**  
Diana Mabel Garcia Martinez  
Universidad Tecnológica del Norte de Guanajuato (UTNG)
