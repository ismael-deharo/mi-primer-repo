# Implementación de Control de Versiones y Despliegue Remoto con Git

**Entorno Técnico:**
- Ubuntu 24.04 LTS
- Git CLI
- Intérprete de comandos Bash

**Objetivo Empresarial:**
Establecer un entorno estandarizado de control de código fuente para garantizar la trazabilidad de los cambios, asegurar el respaldo de los scripts de infraestructura y habilitar la sincronización entre equipos técnicos.

**Implementación y Comandos:**

1. **Aprovisionamiento del software y configuración de identidad**
   ```bash
   sudo apt update
   sudo apt install git -y
   git config --global user.name "Tu Nombre o Alias"
   git config --global user.email "tu-correo@ejemplo.com"

2. **Inicialización del árbol de trabajo local**
   ```bash
   mkdir mi-primer-repo
   cd mi-primer-repo
   echo "# Hola Mundo desde Ubuntu" > README.md
   git init

3. **Indexación y confirmación del estado base (Staging y Commit)**
   ```bash
   git add README.md
   git commit -m "Primer commit: Añadido README inicial"
   git branch -M main

4. **Vinculación con el repositorio centralizado y sincronización (Push)**
   ```bash
   git remote add origin [https://github.com/Tu_Nombre/mi-primer-repo.git](https://github.com/Tu_Nombre/mi-primer-repo.git)
   git remote -v
