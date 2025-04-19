
# 🍌 Banana Ripeness Predictor - Backend

Este es el proyecto **backend** de una aplicación que utiliza **Machine Learning** para predecir el **nivel de madurez de un plátano** a partir de imágenes tomadas diariamente. Este servicio se encarga de recibir imágenes desde el frontend, procesarlas y utilizar un modelo de aprendizaje automático para generar predicciones.

El backend está construido con **Node.js** y el framework **Express**, y expone una API REST para interactuar con el frontend desarrollado en Angular.

---

## ⚙️ Funcionalidades principales

- 📥 Recepción de imágenes desde el cliente.
- 🧠 Procesamiento de imágenes y predicción con modelo de Machine Learning.
- 📊 Envío de resultados al frontend.
- 🗂️ Organización de imágenes por espécimen.
- (Opcional futuro) Autenticación de usuarios.

---

## 🚀 Tecnologías utilizadas

- **Node.js** – Entorno de ejecución para JavaScript en el servidor.
- **Express** – Framework para construcción de APIs REST.
- **TensorFlow.js** / **Python Shell** – Para ejecutar el modelo de predicción (según integración).
- **Multer** – Middleware para manejo de archivos (uploads).
- **Dotenv** – Manejo de variables de entorno.
- **CORS** – Habilitación de comunicación con el frontend.

---

## 📁 Estructura del proyecto

```
banana-ripeness-backend/
├── src/
│   ├── controllers/       # Lógica de negocio y manejo de rutas
│   ├── routes/            # Definición de endpoints de la API
│   ├── services/          # Lógica para llamar al modelo de ML
│   ├── uploads/           # Carpeta para imágenes subidas temporalmente
│   └── app.js             # Configuración principal de Express
├── .env                   # Variables de entorno
├── package.json           # Dependencias del proyecto
└── README.md
```

---

## 🔧 Instalación

### 1. Clona el repositorio

```bash
git clone https://github.com/tu-usuario/banana-ripeness-backend.git
cd banana-ripeness-backend
```

### 2. Instala las dependencias

```bash
npm install
```

### 3. Crea un archivo `.env`

Agrega las variables necesarias. Ejemplo:

```
PORT=3000
MODEL_PATH=./modelo/modelo_platano.h5
```

### 4. Inicia el servidor

```bash
npm start
```

El backend estará disponible en `http://localhost:3000/`.

---

## 📦 Endpoints principales

- `POST /api/predict` – Recibe una imagen y retorna el estado de madurez.
- `GET /api/status` – Verifica si el servidor está corriendo.
- (Opcional futuro) `GET /api/history/:specimenId` – Histórico de predicciones por espécimen.

---

## 🧪 Testing

Puedes probar los endpoints con herramientas como **Postman** o **cURL**. Asegúrate de enviar la imagen como `form-data`.

---

## 📝 Estado del proyecto

- [x] API básica con Express
- [x] Subida de imágenes
- [x] Conexión al modelo de ML
- [x] Predicción y respuesta al cliente
- [ ] Historial por espécimen
- [ ] Seguridad y autenticación

---

## 📄 Licencia

Este proyecto se distribuye bajo la licencia [MIT](LICENSE).
