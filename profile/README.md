# Zeni: Virtual Assistant App

## **Descripción del Proyecto**
Zeni es una aplicación de asistente virtual diseñada para facilitar tareas administrativas y personales, como:
- Gestión de llamadas.
- Manejo de calendarios (Outlook y Google).
- Procesamiento de voz a texto y toma de decisiones basadas en comandos.
- Ejecución de acciones como agendar citas y enlazar llamadas.

El objetivo principal es ofrecer un asistente embebido en un dispositivo y una aplicación móvil sin costos recurrentes para el cliente por el uso del software.

---

## **Organización del Proyecto**

### **1. Funcionalidades Principales**

#### **1.1 Reconocimiento de Voz**
- Utilizar el modelo **Whisper** (OpenAI) implementado a través de la librería Transformers de Hugging Face.
- Procesar comandos de voz en tiempo real para convertirlos en texto.

#### **1.2 Procesamiento de Texto (NLP)**
- Usar modelos preentrenados como **T5** o **GPT** para interpretar las intenciones del usuario.
- Responder a comandos como:
  - "Agendar una cita."
  - "Llamar a Juan."
  - "¿Qué tengo programado hoy?"

#### **1.3 Gestión de Llamadas**
- Configurar una API personalizada o utilizar servicios como Twilio para:
  - Realizar llamadas.
  - Enlazar llamadas entrantes y salientes.
- Alternar entre el uso de la línea del dispositivo Zeni o la del teléfono vinculado.

#### **1.4 Integración con Calendarios**
- Soporte para Google Calendar y Outlook a través de:
  - Google Calendar API.
  - Microsoft Graph API.
- Permitir la autenticación con OAuth 2.0 para gestionar eventos.

#### **1.5 Actualizaciones del Software**
- El asistente estará conectado a internet para descargar actualizaciones periódicas y mantener la experiencia del usuario.

---

### **2. Tecnologías y Herramientas**

#### **2.1 Backend**
- Lenguaje: **Python**
- Frameworks:
  - **Flask** o **FastAPI** (para APIs REST).
- Bases de Datos:
  - **PostgreSQL** (almacenamiento de usuarios y configuraciones).

#### **2.2 Frontend (App Móvil)**
- Tecnologías:
  - **Flutter** (compatibilidad con Android e iOS).
- Funcionalidades:
  - Pantalla de inicio con accesos rápidos.
  - Sincronización con el dispositivo Zeni.
  - Gestión de permisos para llamadas y calendario.

#### **2.3 IA y Modelos**
- **Hugging Face Transformers**:
  - Modelo Whisper para voz a texto.
  - T5 o GPT para procesamiento de texto.
- Framework de Machine Learning:
  - **PyTorch** o **TensorFlow Lite** para despliegue en hardware.

#### **2.4 Telefonía y Conexión**
- Servicios como Twilio o Vonage para llamadas API.
- Configuración de módulos GSM si el hardware soporta chip SIM.

---

### **3. Organización del Desarrollo**

#### **3.1 Etapa 1: MVP (Producto Mínimo Viable)**
- **Duración Estimada**: 2-3 meses.
- Componentes:
  1. Reconocimiento de voz (Whisper).
  2. Procesamiento básico de comandos (T5 o GPT).
  3. App móvil con integración a llamadas y calendarios.
- Objetivo: Probar funcionalidad básica y recopilar retroalimentación inicial.

#### **3.2 Etapa 2: Integración Avanzada**
- **Duración Estimada**: 3-4 meses.
- Componentes:
  1. Implementación completa de la API de telefonía.
  2. Soporte para múltiples idiomas y personalización de comandos.
  3. Optimización de la sincronización entre hardware y app.

#### **3.3 Etapa 3: Despliegue y Escalabilidad**
- **Duración Estimada**: 2 meses.
- Actividades:
  - Implementar actualizaciones OTA (Over-The-Air).
  - Asegurar escalabilidad del backend para manejar usuarios concurrentes.

---

### **4. Consideraciones de Costos**
- **Infraestructura Inicial**:
  - Servidores en la nube (Google Cloud, AWS o Azure): $100 - $500/mes.
- **Desarrollo**:
  - Equipo de 3-5 desarrolladores (app móvil, backend y modelos).
  - Presupuesto inicial: $20,000 - $50,000 USD.

---

### **5. Roadmap**
- **Mes 1**:
  - Configuración del entorno de desarrollo.
  - Implementación inicial de Whisper y Hugging Face.
- **Mes 2-3**:
  - Desarrollo del backend y app móvil MVP.
  - Pruebas de funcionalidad básica.
- **Mes 4-6**:
  - Integración avanzada (telefonía y calendarios).
  - Pruebas beta con usuarios.
- **Mes 7**:
  - Lanzamiento oficial del producto.
  - Recolección de retroalimentación y actualizaciones iniciales.

---

## **Cómo Contribuir**
1. Clona este repositorio y configura el entorno de desarrollo:
   ```bash
   git clone https://github.com/tu-repo/zeni.git
   cd zeni
   ```
2. Instala las dependencias necesarias:
   ```bash
   pip install -r requirements.txt
   ```
3. Asegúrate de tener las credenciales necesarias para APIs externas.

---

## **Licencia**
Este proyecto está bajo la licencia [MIT](LICENSE).

