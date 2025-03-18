# Readme Grupo 4
## Introducción
Trivy es una herramienta que permite escánear vulnerabilidades de codigo de imagenes contenedoras.

## Justificación Técnica

### 1. Escaneo Rápido
Trivy es conocido por su velocidad y precisión en la detección de vulnerabilidades, minimizando los falsos positivos que pueden afectar la confianza de los usuarios en las herramientas de seguridad

### 2. Actualizaciones continuas de la DB
Trivy actualiza regularmente su base de datos de vulnerabilidades lo que proporciona información de seguridad más reciente para un escaneo mas efectivo. Esto es crucial para identificar y mitigar amenzas emergentes de manera proactiva.

### 3. Soporte multientono
Es versatil y puede escanear contenedores, sistemas de archivos, repositorios de código y configuraciones de infraestructura. Esta versatilidad permite una detección exhaustiva de vulnerabilidades en múltiples componenetes del entorno de desarrollo y producción

### 4. Integración CI/CD
Está diseñado teniendo en cuenta la automatización, trivy integra sin problemas en las canalización de CI/CD, lo que permite comprobaciones de seguridad en los flujos de trabajo de desarrollo. Además, su rapidez en el escaneo permite integrarlo eficientemente en las canalizaciones de CI/CD sin compormeter los tiempos de entrega.

## Referencias
- CloudThat. (2024). Detecting and Fixing Vulnerabilities in Docker Images with Trivy and Best Practices. Recuperado de https://www.cloudthat.com/resources/blog/detecting-and-fixing-vulnerabilities-in-docker-images-with-trivy-and-best-practices
- Trivy. Ecosystem. Recuperado de https://trivy.dev/v0.59/ecosystem/
- Aqua. (2021). Trivy´s Journey: From personal project to Open Source Scanner of Choice. Recuperado de https://www.aquasec.com/blog/trivy-scanner/
- Medium. (2024). Catching Vulnerabilities in Your Docker Images: The Power of trivy. Recuperado de https://medium.com/%40sachinsoni600517/catching-vulnerabilities-in-your-docker-images-the-power-of-trivy-6c86494b0564
