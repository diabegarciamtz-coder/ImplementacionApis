# Simple Flask API 🚀

Pequeña API desarrollada con **Python** usando el framework **:contentReference[oaicite:0]{index=0}** para practicar la creación de endpoints y probar peticiones HTTP con **:contentReference[oaicite:1]{index=1}**.

---

## 📌 Descripción

Este proyecto implementa una API básica que permite:

- Obtener información de un usuario por su **ID**
- Crear un usuario enviando datos en **JSON**
- Probar endpoints utilizando herramientas de testing de APIs

Es un proyecto pequeño pensado para practicar el funcionamiento básico de una API REST.

---

## 🛠 Tecnologías utilizadas

- Python 3
- Flask
- Postman

---

## 📂 Estructura del proyecto

```
implementacionapi
│
├── main.py
├── README.md
└── venv/   (entorno virtual - no se sube al repositorio)
```


### Respuesta de la API

<img width="1918" height="1079" alt="image" src="https://github.com/user-attachments/assets/4795d281-e362-401a-beed-f863b1c22fcb" />
<img width="1919" height="1079" alt="image" src="https://github.com/user-attachments/assets/a3b568d7-275e-4a41-9d21-16fc68ba2963" />
<img width="1919" height="1078" alt="image" src="https://github.com/user-attachments/assets/c5cc41da-6ed6-4981-9be2-dc1fef56dc15" />

---

## ▶️ Cómo ejecutar el proyecto

### 1. Clonar el repositorio

```
git clone https://github.com/TU_USUARIO/TU_REPOSITORIO.git
```

### 2. Entrar a la carpeta del proyecto

```
cd implementacionapi
```

### 3. Crear entorno virtual

```
python -m venv venv
```

### 4. Activar entorno virtual

Windows (PowerShell)

```
.\venv\Scripts\Activate.ps1
```

Linux / Mac

```
source venv/bin/activate
```

### 5. Instalar dependencias

```
pip install flask
```

### 6. Ejecutar la aplicación

```
python main.py
```

La API se ejecutará en:

```
http://127.0.0.1:5000
```

---

## 🔗 Endpoints disponibles

### GET /users/<user_id>

Obtiene un usuario por su ID.

Ejemplo:

```
GET http://127.0.0.1:5000/users/20
```

Respuesta:

```json
{
"id": "20",
"name": "test",
"telefono": "999-666-333"
}
```

También permite query params:

```
GET /users/20?query=test
```

---

### POST /users

Crea un usuario enviando datos en formato JSON.

Ejemplo de request en Postman:

```
POST http://127.0.0.1:5000/users
```

Body:

```json
{
"id": "20",
"name": "Brenda",
"telefono": "418-114-9982"
}
```

Respuesta:

```json
{
"id": "20",
"name": "Brenda",
"telefono": "418-114-9982",
"status": "user created"
}
```

---

## 🧪 Pruebas

Los endpoints fueron probados usando **Postman** enviando peticiones HTTP **GET** y **POST**.

---

## 📚 Aprendizaje del ejercicio

Este ejercicio tuve como objetivo entender los fundamentos de cómo funciona una **API REST** utilizando **Python y Flask**. 
A través de la creación de endpoints practiqué con  la definición de rutas, el uso de
*query parameters*, la recepción de datos en formato **JSON** mediante peticiones **POST**, y el envío de respuestas en formato
JSON desde el servidor. Además, se utilizó **:contentReference[oaicite:0]{index=0}** para probar las peticiones HTTP y verificar el
funcionamiento de la API desarrollada con **:contentReference[oaicite:1]{index=1}**.

## 📄 Licencia

---

Este proyecto es solo para fines educativos y de práctica.
Brenda Edith Grifaldo Delgadillo
UTNG®
