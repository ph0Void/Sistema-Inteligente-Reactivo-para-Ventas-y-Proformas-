# ⚡ SmartSales — Sistema Reactivo Inteligente para Ventas y Proformas

🚀 SmartSales  es un sistema moderno y escalable desarrollada bajo una arquitectura de **microservicios reactivos**, impulsada por **Spring Boot WebFlux** en el backend y **Next.js** en el frontend.
Diseñada para ofrecer rendimiento, eficiencia y una experiencia inteligente, permite la gestión completa de productos, ventas, clientes y proformas, con generación automática de recibos y proformas en formato PDF.

💡 Además, integra un **asistente conversacional inteligente** (chatbot) basado en Spring AI, que conecta con modelos locales a través de LM Studio + Qwen3, 
brindando soporte contextual, respuestas personalizadas y facilitando los procesos comerciales.

---
<img width="4985" height="2419" alt="PROYCETOS MSVC" src="https://github.com/user-attachments/assets/428235d3-4f3e-4ecc-bd74-2e4de2f8b40b" />



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

| Servicio | Descripción | Puerto |
|-----------|--------------|--------|
| **msvc-auth** | Autenticación y gestión de usuarios (JWT + MongoDB) | 8083 |
| **msvc-products** | CRUD de productos con MongoDB reactivo | 8081 |
| **msvc-customer** | Gestión de clientes y vendedores | 8082 |
| **msvc-sales** | Orquestación de ventas / proformas | 8085 |
| **msvc-images** | Subida y gestión de imágenes con Cloudinary | 8084 |
| **msvc-chatbot** | Asistente virtual (Spring AI + LM Studio + Qwen3) | 8086 |
| **msvc-gateway** | API Gateway / seguridad / enrutamiento | 8080 |

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

<img width="800" height="600" alt="image" src="https://github.com/user-attachments/assets/22a5d984-1145-4e82-ba02-ad66f4f16980" />

<img width="800" height="600" alt="image" src="https://github.com/user-attachments/assets/f45d5920-88b6-48e5-b8aa-277c0dfceaa1" />
<img width="800" height="600" alt="image" src="https://github.com/user-attachments/assets/cf1e6dd1-0f4c-47ba-937f-9030f62bca0f" />

<img width="800" height="600" alt="image" src="https://github.com/user-attachments/assets/76543c7e-6128-41c3-a9d8-57a91922d4d2" />


<img width="800" height="600" alt="image" src="https://github.com/user-attachments/assets/04768a28-4755-4793-b5dc-853ed77470ae" />

<img width="800" height="600" alt="image" src="https://github.com/user-attachments/assets/76b1d90e-f893-43de-831f-070fd193c0c1" />
<img width="800" height="600" alt="image" src="https://github.com/user-attachments/assets/dc7ef5a1-af8b-436f-9361-6144087fb468" />


---
