# 📹 TechInsight Video Uploader

Esta aplicación Spring Boot permite a los usuarios subir vídeos directamente a un bucket de AWS S3 mediante un método POST.

## ⚙️ Configuración

Antes de ejecutar la aplicación, es necesario configurar las siguientes propiedades en tu archivo `application.properties`. Asegúrate de modificar los valores según tus necesidades y tu cuenta de AWS.

```properties
# Nombre de la aplicación Spring
spring.application.name=techinsight

# Credenciales de AWS
aws.accessKeyId={ TU ACCESS KEY ID }
aws.secretKey={ TU SECRET KEY }

# Configuración de S3
aws.s3.bucket={ TU BUCKET }
aws.region=us-east-2

# Configuración de carga de archivos
spring.servlet.multipart.max-file-size=200MB
spring.servlet.multipart.max-request-size=200MB
```

# 🚀 Ejecución
Para ejecutar la aplicación, utiliza el siguiente comando:


Copiar código
```bash
./mvnw spring-boot:run
```
Tambien puedes hacer funcionar la aplicacion utilizando un editor de codigo como Intellij con jdk 17

# 📤 Uso
Para subir un video, puedes usar una herramienta como Postman de la siguiente manera:

![SolicitudPostman](https://github.com/mndiazf/techInsights/assets/110750463/9ff6f0df-5cd5-4d8f-874b-7e334b2a59b4)

# 🛠️ Tecnologías utilizadas
Spring Boot
AWS SDK for Java
JDK 17
Maven

# 🔒 Seguridad
Asegúrate de no subir tus credenciales de AWS a repositorios públicos para evitar el acceso no autorizado a tus recursos de AWS.
