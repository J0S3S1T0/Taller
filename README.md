 # 🚗 Viaggio Velogge — API y Frontend de Autos y Accesorios

> Una aplicación full-stack moderna con autenticación segura, gestión de autos, accesorios y carritos de compra.  
> Backend: FastAPI + MySQL | Frontend: Next.js 15 + TypeScript

![Viaggio Velogge](https://via.placeholder.com/800x400?text=Viaggio+Velogge+Logo) <!-- Puedes reemplazar esto por una imagen real más  -->

---

## 📌 Tabla de Contenidos

- [🔧 Requisitos](#-requisitos)
- [🚀 Instalación del Proyecto](#-instalación-del-proyecto)
- [⚙️ Configuración del Backend (FastAPI)](#️-configuración-del-backend-fastapi)
- [🌐 Configuración del Frontend (Next.js)](#-configuración-del-frontend-nextjs)
- [🔐 Variables de Entorno (.env)](#-variables-de-entorno-env)
- [💾 Base de Datos (MySQL)](#-base-de-datos-mysql)
- [🧪 Pruebas y Uso](#-pruebas-y-uso)
- [📂 Estructura del Proyecto](#-estructura-del-proyecto)
- [🧩 Contribuciones](#-contribuciones)
- [📜 Licencia](#-licencia)

---

## 🔧 Requisitos

Antes de comenzar, asegúrate de tener instalado:

| Herramienta | Versión Recomendada |
|------------|---------------------|
| Node.js | v18.x o superior |
| Python | v3.9 – v3.12 |
| MySQL | v8.0+ |
| Git | Última versión |

> 💡 Recomendamos usar **VS Code** como editor y **HeidiSQL** o **DBeaver** para gestionar MySQL.

---

## 🚀 Instalación del Proyecto

Clona el repositorio:

```bash
git clone https://github.com/tuusuario/viaggio-velogge.git
cd viaggio-velogge


cd backend
python -m venv venv
source venv/bin/activate    # Linux/Mac
# O en Windows:
venv\Scripts\activate



pip install fastapi uvicorn sqlalchemy pymysql passlib[bcrypt] python-jose[cryptography] python-dotenv



CREATE DATABASE ViaggioVelogge CHARACTER SET utf8mb4 COLLATE utf8mb4_unicode_ci;
USE ViaggioVelogge;


cp .env.example .env

uvicorn main:app --reload --host 0.0.0.0 --port 8000
http://localhost:8000/docs




cd ../frontend
npm install

cp .env.local.example .env.local
NEXT_PUBLIC_API_URL=http://localhost:8000/api/v1
npm run dev




# Inicializa git
git init

# Añade el .gitignore
git add .gitignore

# Añade tu .env.example (NO .env!)
git add .env.example

# Añade todo lo demás (código fuente)
git add backend/ frontend/

# Haz tu primer commit
git commit -m "feat: initial project structure with FastAPI + Next.js"

# Ahora puedes conectar a GitHub
git remote add origin https://github.com/tuusuario/viaggio-velogge.git
git branch -M main
git push -u origin main
