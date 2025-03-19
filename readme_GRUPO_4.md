# Readme Grupo 4
## Introducción
Trivy es una herramienta que permite escánear vulnerabilidades de codigo de imagenes contenedoras.

## Descripcion
Trivy es un escáner de seguridad integral y versátil desarrollado por Aqua Security. Está diseñado para identificar vulnerabilidades y problemas de configuración en una amplia gama de objetivos, incluyendo imágenes de contenedores, sistemas de archivos, repositorios de código, máquinas virtuales, clústeres de Kubernetes y entornos en la nube. 

## Funcionalidades principales

### •	Escaneo de imágenes de contenedores
Trivy analiza imágenes de contenedores en busca de vulnerabilidades conocidas en paquetes del sistema operativo y dependencias de aplicaciones. Soporta múltiples sistemas operativos y gestores de paquetes, como Alpine, RHEL, CentOS, Debian, Ubuntu, npm, yarn, entre otros. 

### •	Análisis de sistemas de archivos y repositorios de código
Permite escanear sistemas de archivos locales y repositorios de código (tanto locales como remotos) para detectar vulnerabilidades en dependencias y configuraciones. Es compatible con diversos lenguajes y entornos de desarrollo. 

### •	Detección de problemas de configuración y secretos
Identifica problemas de configuración en infraestructuras como código (IaC) y busca información sensible o secretos que puedan estar expuestos en el código o en la configuración. 

### •	Análisis de licencias de software
Trivy evalúa las licencias de las dependencias utilizadas, ayudando a garantizar el cumplimiento con las políticas de licencias y evitando posibles conflictos legales. 

### •	Operador Trivy para Kubernetes
El Trivy Operator extiende las capacidades de Trivy al entorno de Kubernetes, realizando escaneos continuos de seguridad en clústeres y generando informes detallados sobre los recursos y configuraciones.  

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
- Trivy Operator. (2022).Recuperado de https://aquasecurity.github.io/trivy-operator/latest/
- Aquasecurity. Trivy. Recuperado de https://github.com/aquasecurity/trivy
- Trivy. Repositorio de codigo. Recuperado de https: https://trivy.dev/latest/docs/target/repository/
- CloudThat. (2024). Detecting and Fixing Vulnerabilities in Docker Images with Trivy and Best Practices. Recuperado de https://www.cloudthat.com/resources/blog/detecting-and-fixing-vulnerabilities-in-docker-images-with-trivy-and-best-practices
- Trivy. Ecosystem. Recuperado de https://trivy.dev/v0.59/ecosystem/
- Medium. (2024). Catching Vulnerabilities in Your Docker Images: The Power of trivy. Recuperado de https://medium.com/%40sachinsoni600517/catching-vulnerabilities-in-your-docker-images-the-power-of-trivy-6c86494b0564
