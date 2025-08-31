# 🔶 Intermedio 2 - Documentación de API

## 🧭 Navegación del Curso

- **⬅️ Anterior**: [Módulo 4: Revisiones de Código](../intermediate_1/README.md)
- **➡️ Siguiente**: [Módulo 6: Comunicación en Equipos](../intermediate_3/README.md)
- **📚 [Índice Completo](../INDICE_COMPLETO.md)** | **[🧭 Navegación Rápida](../NAVEGACION_RAPIDA.md)**

---

## 📚 **Descripción del Nivel**

¡Bienvenido al segundo nivel intermedio! Ahora aprenderás a crear documentación técnica profesional en inglés, especialmente para APIs. Este nivel te preparará para escribir documentación que sea clara, completa y útil para desarrolladores de todo el mundo.

**IMPORTANTE**: En este nivel, el inglés se convierte en tu herramienta principal de comunicación técnica, pero siempre con explicaciones claras y ejemplos prácticos.

## 🎯 **Contenido Principal**

### 1. **Vocabulario de Documentación Técnica**

#### **Términos de Documentación**
```markdown
# Vocabulario de Documentación

## Tipos de Documentación
- **API reference** (se pronuncia: "éi-pi-ái réferens") = referencia de API (documentación completa de endpoints)
- **user guide** (se pronuncia: "iúser gaid") = guía de usuario (instrucciones paso a paso)
- **tutorial** (se pronuncia: "tiutórial") = tutorial (aprendizaje guiado)
- **getting started** (se pronuncia: "gueting stárted") = comenzando (primeros pasos)
- **examples** (se pronuncia: "igzámpols") = ejemplos (casos de uso prácticos)

## Elementos de Documentación
- **endpoint** (se pronuncia: "éndpoint") = punto final (URL de la API)
- **request** (se pronuncia: "rikwést") = solicitud (datos enviados al servidor)
- **response** (se pronuncia: "rispóns") = respuesta (datos devueltos por el servidor)
- **authentication** (se pronuncia: "otentikéishon") = autenticación (verificación de identidad)
- **authorization** (se pronuncia: "otoraizéishon") = autorización (permisos de acceso)
```

#### **Términos de Escritura Técnica**
```markdown
# Vocabulario de Escritura

## Estructura y Organización
- **overview** (se pronuncia: "óverviu") = vista general (resumen del contenido)
- **prerequisites** (se pronuncia: "prikwiérisits") = prerrequisitos (lo que necesitas antes de empezar)
- **step-by-step** (se pronuncia: "stép-bai-stép") = paso a paso (instrucciones secuenciales)
- **troubleshooting** (se pronuncia: "trábolshuting") = solución de problemas (resolver errores comunes)
- **best practices** (se pronuncia: "best práktisis") = mejores prácticas (recomendaciones)
```

### 2. **Estructura de Documentación de API**

#### **Formato Estándar de Endpoint**
```markdown
# Estructura de Documentación de API

## Ejemplo Completo

### **POST /api/users**
Create a new user in the system = Crear un nuevo usuario en el sistema

**Description** = Descripción
This endpoint allows you to create a new user account with the provided information. = Este endpoint te permite crear una nueva cuenta de usuario con la información proporcionada.

**Authentication** = Autenticación
Required = Requerido: Bearer token in Authorization header = Token Bearer en el encabezado de Autorización

**Request Body** = Cuerpo de la Solicitud
```json
{
  "username": "string",
  "email": "string",
  "password": "string",
  "firstName": "string",
  "lastName": "string"
}
```

**Parameters** = Parámetros
- **username** (string, required) = nombre de usuario (cadena, requerido): Unique login name = Nombre de inicio de sesión único
- **email** (string, required) = email (cadena, requerido): Valid email address = Dirección de email válida
- **password** (string, required) = contraseña (cadena, requerida): Minimum 8 characters = Mínimo 8 caracteres
- **firstName** (string, optional) = nombre (cadena, opcional): User's first name = Nombre del usuario
- **lastName** (string, optional) = apellido (cadena, opcional): User's last name = Apellido del usuario

**Response** = Respuesta
**200 OK** = Usuario creado exitosamente
```json
{
  "id": "12345",
  "username": "john_doe",
  "email": "john@example.com",
  "firstName": "John",
  "lastName": "Doe",
  "createdAt": "2024-01-15T10:30:00Z",
  "status": "active"
}
```

**Error Responses** = Respuestas de Error
**400 Bad Request** = Datos de entrada inválidos
**409 Conflict** = Usuario ya existe
**500 Internal Server Error** = Error interno del servidor
```

#### **Secciones de Documentación Completa**
```markdown
# Secciones de Documentación

## 1. Overview = Vista General
- **What is this API?** = ¿Qué es esta API?
- **Key features** = Características principales
- **Use cases** = Casos de uso

## 2. Getting Started = Comenzando
- **Prerequisites** = Prerrequisitos
- **Installation** = Instalación
- **Quick start** = Inicio rápido

## 3. Authentication = Autenticación
- **API keys** = Claves de API
- **OAuth 2.0** = OAuth 2.0
- **JWT tokens** = Tokens JWT

## 4. Endpoints = Puntos Finales
- **Base URL** = URL base
- **HTTP methods** = Métodos HTTP
- **Response formats** = Formatos de respuesta

## 5. Examples = Ejemplos
- **Basic usage** = Uso básico
- **Advanced scenarios** = Escenarios avanzados
- **Error handling** = Manejo de errores

## 6. SDKs & Libraries = SDKs y Bibliotecas
- **Official SDKs** = SDKs oficiales
- **Community libraries** = Bibliotecas de la comunidad
- **Code samples** = Ejemplos de código
```

### 3. **Escritura Técnica Efectiva**

#### **Principios de Escritura Clara**
```markdown
# Principios de Escritura Técnica

## Claridad y Simplicidad
- **Use simple language** = Usa lenguaje simple: "Create a user" instead of "Instantiate a user entity" = "Crear un usuario" en lugar de "Instanciar una entidad de usuario"
- **Be specific** = Sé específico: "Set the timeout to 30 seconds" instead of "Set an appropriate timeout" = "Establece el timeout a 30 segundos" en lugar de "Establece un timeout apropiado"
- **Avoid jargon** = Evita jerga: "Send data" instead of "Transmit payload" = "Enviar datos" en lugar de "Transmitir carga útil"

## Estructura y Organización
- **Logical flow** = Flujo lógico: Start with basics, then advanced topics = Comienza con lo básico, luego temas avanzados
- **Consistent formatting** = Formato consistente: Use the same style for similar elements = Usa el mismo estilo para elementos similares
- **Clear headings** = Encabezados claros: Make navigation easy = Facilita la navegación
```

#### **Ejemplos de Escritura Técnica**
```markdown
# Ejemplos de Escritura

## ✅ **Buen Ejemplo**
To authenticate with the API, you need to include your API key in the request header. = Para autenticarte con la API, necesitas incluir tu clave de API en el encabezado de la solicitud.

**Steps** = Pasos:
1. Get your API key from the dashboard = Obtén tu clave de API desde el panel
2. Add the key to the Authorization header = Agrega la clave al encabezado de Autorización
3. Send your request = Envía tu solicitud

**Example** = Ejemplo:
```bash
curl -H "Authorization: Bearer YOUR_API_KEY" \
     https://api.example.com/users
```

## ❌ **Mal Ejemplo**
Authentication is required for API access. You must authenticate. = La autenticación es requerida para el acceso a la API. Debes autenticarte.

**Problem** = Problema: Vague instructions, no examples, repetitive language = Instrucciones vagas, sin ejemplos, lenguaje repetitivo
```

### 4. **Documentación de Errores y Solución de Problemas**

#### **Estructura de Documentación de Errores**
```markdown
# Documentación de Errores

## Error Code Reference = Referencia de Códigos de Error

### **400 Bad Request**
**Meaning** = Significado: The request contains invalid data = La solicitud contiene datos inválidos

**Common Causes** = Causas Comunes:
- Missing required fields = Campos requeridos faltantes
- Invalid data format = Formato de datos inválido
- Data validation failed = Falló la validación de datos

**How to Fix** = Cómo Solucionarlo:
1. Check that all required fields are present = Verifica que todos los campos requeridos estén presentes
2. Ensure data format matches the specification = Asegúrate de que el formato de datos coincida con la especificación
3. Validate your data before sending = Valida tus datos antes de enviar

**Example** = Ejemplo:
```json
// ❌ Invalid - missing email
{
  "username": "john_doe",
  "password": "secret123"
}

// ✅ Valid - all required fields present
{
  "username": "john_doe",
  "email": "john@example.com",
  "password": "secret123"
}
```
```

#### **Guía de Solución de Problemas**
```markdown
# Guía de Solución de Problemas

## Common Issues = Problemas Comunes

### **Authentication Failed** = Falló la Autenticación
**Symptoms** = Síntomas: Getting 401 Unauthorized errors = Obtener errores 401 No Autorizado

**Diagnosis** = Diagnóstico:
1. Check if your API key is valid = Verifica si tu clave de API es válida
2. Ensure the key is included in the header = Asegúrate de que la clave esté incluida en el encabezado
3. Verify the key hasn't expired = Verifica que la clave no haya expirado

**Solution** = Solución:
1. Generate a new API key = Genera una nueva clave de API
2. Update your code to use the new key = Actualiza tu código para usar la nueva clave
3. Test with a simple endpoint first = Prueba primero con un endpoint simple

### **Rate Limiting** = Limitación de Tasa
**Symptoms** = Síntomas: Getting 429 Too Many Requests = Obtener 429 Demasiadas Solicitudes

**Diagnosis** = Diagnóstico:
1. Check your current usage = Verifica tu uso actual
2. Review your rate limit = Revisa tu límite de tasa
3. Identify burst requests = Identifica solicitudes en ráfaga

**Solution** = Solución:
1. Implement exponential backoff = Implementa retroceso exponencial
2. Cache responses when possible = Almacena en caché las respuestas cuando sea posible
3. Batch requests together = Agrupa solicitudes juntas
```

## 🧪 **Ejercicios Prácticos**

### **Ejercicio 1: Documentar un Endpoint Completo**
1. **Objetivo**: Crear documentación completa para un endpoint de API
2. **Pasos**:
   - Elige un endpoint de una API existente
   - Documenta todos los aspectos (request, response, errors)
   - Incluye ejemplos de código en múltiples lenguajes
   - Escribe la documentación completamente en inglés

### **Ejercicio 2: Crear Guía de Solución de Problemas**
1. **Objetivo**: Desarrollar documentación de troubleshooting efectiva
2. **Pasos**:
   - Identifica 5 problemas comunes de una API
   - Para cada problema, escribe síntomas, diagnóstico y solución
   - Incluye ejemplos de código para cada solución
   - Organiza la información de manera lógica y fácil de seguir

### **Ejercicio 3: Escribir Tutorial Paso a Paso**
1. **Objetivo**: Crear un tutorial completo para desarrolladores
2. **Pasos**:
   - Elige una funcionalidad compleja de una API
   - Crea un tutorial que guíe desde lo básico hasta lo avanzado
   - Incluye ejemplos prácticos y casos de uso reales
   - Escribe completamente en inglés técnico

### **Ejercicio 4: Documentación de SDK**
1. **Objetivo**: Documentar una biblioteca o SDK
2. **Pasos**:
   - Crea documentación para un SDK ficticio
   - Incluye instalación, configuración y ejemplos de uso
   - Documenta todas las clases y métodos principales
   - Escribe en inglés técnico profesional

### **Ejercicio 5: API Reference Completa**
1. **Objetivo**: Crear una referencia completa de API
2. **Pasos**:
   - Diseña una API completa con 10+ endpoints
   - Documenta cada endpoint siguiendo estándares profesionales
   - Incluye autenticación, manejo de errores y ejemplos
   - Crea documentación que sea fácil de navegar y entender

## 🏗️ **Proyecto Integrador: Documentación de API Completa**

### **Descripción**
Crea una documentación completa y profesional para una API de gestión de música (similar a MussikOn), demostrando todas las habilidades de escritura técnica aprendidas.

### **Características a Implementar**
1. **API Reference**: Documentación completa de todos los endpoints
2. **Getting Started Guide**: Guía de inicio rápido para desarrolladores
3. **Authentication Guide**: Guía completa de autenticación y autorización
4. **Error Handling**: Documentación detallada de errores y soluciones
5. **Code Examples**: Ejemplos en múltiples lenguajes de programación
6. **SDK Documentation**: Documentación de bibliotecas cliente
7. **Tutorials**: Guías paso a paso para casos de uso comunes

### **Entregables**
- Documentación completa de la API en formato web
- Guías de inicio rápido y tutoriales
- Ejemplos de código en JavaScript, Python, C#, y Java
- Documentación de manejo de errores y troubleshooting
- SDK con documentación completa
- Video explicando la API en inglés

## 📋 **Quiz de Evaluación**

### **Pregunta 1**
¿Qué elementos debe incluir la documentación de un endpoint de API?

### **Pregunta 2**
¿Cómo estructurarías una guía de solución de problemas?

### **Pregunta 3**
¿Qué principios seguirías para escribir documentación técnica clara?

### **Pregunta 4**
¿Cómo documentarías diferentes tipos de respuestas de error?

### **Pregunta 5**
¿Qué secciones incluirías en una documentación completa de API?

## 🔗 **Navegación**

### **🔶 Anterior**
- [Intermedio 1 - Revisiones de Código y Discusiones Técnicas](../intermediate_1/README.md)

### **🔶 Siguiente**
- [Intermedio 3 - Comunicación en Equipos Internacionales](../intermediate_3/README.md)

## 📖 **Recursos Adicionales**

### **Herramientas de Documentación**
- **Swagger/OpenAPI**: Estándar para documentación de API
- **Postman**: Documentación interactiva de API
- **GitBook**: Plataforma de documentación técnica
- **ReadTheDocs**: Hosting de documentación técnica

### **Estándares y Mejores Prácticas**
- **OpenAPI Specification**: Especificación estándar para APIs
- **Microsoft Writing Style Guide**: Guía de estilo de Microsoft
- **Google Developer Documentation**: Documentación de desarrolladores de Google
- **Stripe API Documentation**: Ejemplo de excelente documentación de API

### **Recursos de Aprendizaje**
- **Technical Writing Courses**: Cursos de escritura técnica
- **API Design Best Practices**: Mejores prácticas de diseño de API
- **Documentation Tools**: Herramientas de documentación
- **User Experience in Documentation**: Experiencia de usuario en documentación

---

**🎉 ¡Felicitaciones! Has completado el Nivel Intermedio 2!**

**Próximo Paso**: [Intermedio 3 - Comunicación en Equipos Internacionales](../intermediate_3/README.md)

---

**Recuerda**: La documentación técnica es la cara pública de tu código. Una documentación bien escrita puede hacer que tu API sea adoptada por miles de desarrolladores, mientras que una documentación pobre puede hacer que sea ignorada por completo. El inglés técnico es tu herramienta para conectar con desarrolladores de todo el mundo.

