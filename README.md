# ⚡ Sistema Reactivo Inteligente para Ventas y Proformas

🚀 SmartSales  es un sistema moderno y escalable desarrollada bajo una arquitectura de **microservicios reactivos**, impulsada por **Spring Boot WebFlux** en el backend y **Next.js** en el frontend.
Diseñada para ofrecer rendimiento, eficiencia y una experiencia inteligente, permite la gestión completa de productos, ventas, clientes y proformas, con generación automática de recibos y proformas en formato PDF.

💡 Además, integra un **asistente conversacional inteligente** (chatbot) basado en Spring AI, que conecta con modelos locales a través de LM Studio + Qwen3, 
brindando soporte contextual, respuestas personalizadas y facilitando los procesos comerciales.

---
<img width="1000" height="900" alt="0- diagrama " src="https://github.com/user-attachments/assets/dc37b8c3-0813-4994-aada-297f3ec5e0ce" />


<img width="1000" height="900" alt="3 -dashboard" src="https://github.com/user-attachments/assets/80b41383-0a73-4de2-bede-50dba893080c" />

## 🧩 Descripción general

**SmartSales AI Platform** es una aplicación que implementa una arquitectura de **microservicios**, comunicados entre sí mediante **Spring WebClient** y asegurados a través de **Spring Cloud Gateway** con autenticación JWT.

El backend (Spring Boot) ofrece servicios especializados:
- Gestión de productos, clientes, vendedores, imágenes y ventas.
- Módulo de autenticación (Auth Service).
- Chatbot inteligente integrado con **Spring AI**.
- Gateway para seguridad y enrutamiento centralizado.

El frontend (Next.js + TypeScript) consume los servicios mediante API REST, brindando una interfaz moderna, rápida y responsiva con dashboards, proformas descargables en PDF y un asistente de chat contextual.

---

## 🧠 Arquitectura general

- **Frontend:** Next.js + TypeScript + TailwindCSS  
- **Backend:** Spring Boot WebFlux (microservicios reactivas con MongoDB)
- **Gateway:** Spring Cloud Gateway + JWT  
- **Base de datos:** MongoDB (persistencia reactiva)
- **IA:** Spring AI + LM Studio + Qwen3 (Chatbot)
- **Cloud Storage:** Cloudinary (gestión de imágenes)

---

## 🛠️ Tecnologías principales

### Backend
- ☕ **Java 25**
- ⚙️ **Spring Boot 3.x**
- 🌐 **Spring WebFlux** (reactivo)
- 🔐 **Spring Security + JWT**
- 🚀 **Spring Cloud Gateway**
- 🌱 **Spring Data MongoDB Reactive**
- 🔗 **Spring WebClient** (comunicación entre microservicios)
- 🤖 **Spring AI** (integración con modelos locales / externos)
- 📘 **SpringDoc OpenAPI**
- ☁️ **Cloudinary SDK**
- 🧩 **Project Reactor / Lombok / Maven Multimodule**

### Frontend
- ⚛️ **Next.js 15 (Turbopack)**
- 💙 **TypeScript**
- 🎨 **Tailwind CSS**
- 🧠 **Zustand** (estado global con persistencia)
- 📊 **Chart.js + react-chartjs-2**
- 🧾 **@react-pdf/renderer** (PDFs)
- 💬 **react-markdown + remark-gfm**
- ✅ **Zod** (validación de esquemas)
- 🔔 **Sonner (toasts)**

---

## ⚡ Microservicios del sistema


| Microservicio      | Nombre de la aplicación | Puerto | Ruta base ejemplo |
|--------------------|-------------------------|--------:|-------------------|
| API Gateway        | msvc-gateway            |   8080 | http://localhost:8080/ |
| Productos          | msvc-product            |   8081 | http://localhost:8081/products |
| Clientes           | msvc-customer           |   8082 | http://localhost:8082/customers |
| Autenticación      | msvc-authorization      |   8083 | http://localhost:8083/auth |
| Imágenes           | msvc-images             |   8084 | http://localhost:8084/images |
| Ventas/Proformas   | msvc-sales              |   8085 | http://localhost:8085/sales |
| Chatbot            | msvc-chatbot            |   8086 | http://localhost:8086/chatbot |
| Eureka Server      | msvc-eurekaServer       |  8761 | http://localhost:8761/ |

---

## 💡 Funcionalidades principales

### 🔙 Backend
- 🔐 **Autenticación JWT** centralizada en el gateway.
- 🧾 **CRUD reactivo de productos**, clientes y ventas.
- ☁️ **Subida de imágenes** a Cloudinary.
- 🧠 **Chatbot inteligente** conectado con Spring AI.
- 📡 **Comunicación no bloqueante** entre microservicios (WebClient).
- 📘 **Documentación automática OpenAPI.**
- ⚙️ **Gestión modular** mediante Maven multi-módulo.

### 💻 Frontend
- 📦 **Gestión completa de productos, clientes y ventas.**
- 🧾 **Generación de proformas y facturas en PDF.**
- 📈 **Dashboard con métricas y gráficos.**
- 💬 **Chatbot con persistencia de conversación local.**
- 🔒 **Login y registro de usuarios con JWT.**
- 🧩 **Interfaz responsive y modular (Tailwind + componentes reutilizables).**

---

## ✨ Características destacadas

- 🔄 **Arquitectura desacoplada por microservicios.**
- ⚡ **WebFlux y MongoDB reactivo** para rendimiento y escalabilidad.
- 🧠 **Spring AI** para potenciar un chatbot contextual que accede a datos del sistema.
- ☁️ **Cloudinary** para almacenamiento de imágenes.
- 🔐 **Seguridad centralizada con Spring Cloud Gateway + JWT.**
- 📦 **Frontend moderno con Next.js + Zustand + Zod.**
- 🧾 **PDFs de proformas generados en el cliente.**
- 📘 **Documentación automática (Swagger / OpenAPI).**

---
## Imagenes 

<img width="1000" height="900" alt="1-login" src="https://github.com/user-attachments/assets/bf75e520-6fb9-43b6-a214-e9694207b61f" />


<img width="1000" height="900" alt="2 - home" src="https://github.com/user-attachments/assets/d88ae1a3-2fda-4028-ae1d-5bc743102c2a" />

<img width="1000" height="900" alt="3 - perfil usuario " src="https://github.com/user-attachments/assets/322f986e-4c2e-4df8-ae6a-c14c80537e39" />
<img width="1000" height="900" alt="3 -dashboard" src="https://github.com/user-attachments/assets/e5009178-742f-4a4a-bf4a-314b6d1d1191" />

<img width="1000" height="900" alt="4 - productos" src="https://github.com/user-attachments/assets/863ecd99-15d0-4ad6-8dde-0c165e6f9582" />
<img width="1000" height="900" alt="5 carrito de compras" src="https://github.com/user-attachments/assets/e90ca826-9777-4e2c-8193-88e5300e57cb" />

<img width="1000" height="900" alt="6 - generacoin de la orden " src="https://github.com/user-attachments/assets/1cf2ce85-6b2f-4d4a-95ab-2450cdde39d6" />

<img width="1000" height="900" alt="7 tabla de compras" src="https://github.com/user-attachments/assets/511be8b1-9632-44cd-b792-b8573a4bdfd9" />

<img width="1000" height="900" alt="8 boleta de venta " src="https://github.com/user-attachments/assets/def200aa-9469-4962-bcb7-c082318806c1" />

<img width="1000" height="900" alt="9 exportacion de pdf " src="https://github.com/user-attachments/assets/c231ccdb-b1dc-4640-9fa2-ec10a12d4625" />
