# Despliegue de una Máquina Virtual en Azure

Este documento proporciona una guía paso a paso para desplegar una máquina virtual (VM) en el portal de Azure. 

## Requisitos Previos

Antes de comenzar, asegúrate de cumplir con los siguientes requisitos:

- Tener una cuenta de Microsoft Azure. Si no tienes una, puedes crear una en [Azure Portal](https://portal.azure.com).
- Acceso al portal de Azure.

## Pasos para Desplegar una Máquina Virtual en Azure

### 1. Iniciar Sesión en el Portal de Azure

1. Ve al [Portal de Azure](https://portal.azure.com).
2. Inicia sesión con tus credenciales de Azure.

### 2. Crear una Máquina Virtual

1. En el panel de navegación izquierdo, selecciona **"Máquinas virtuales"**.
2. Haz clic en **"Crear"** y luego selecciona **"Máquina virtual de Azure"**.

### 3. Configurar los Detalles Básicos de la Máquina Virtual

Rellena la información requerida en la pestaña **"Básico"**:

- **Suscripción**: Selecciona tu suscripción de Azure.
- **Grupo de recursos**: Elige un grupo de recursos existente o crea uno nuevo.
- **Nombre de la máquina virtual**: Introduce un nombre para la VM.
- **Región**: Selecciona la región donde deseas desplegar la VM.
- **Opciones de disponibilidad**: Selecciona una opción basada en tus necesidades de disponibilidad.
- **Imagen**: Elige el sistema operativo de la VM (por ejemplo, "Ubuntu Server 20.04 LTS").
- **Tamaño**: Selecciona el tamaño de la VM (CPU, RAM).

![](/imgs/Captura%20de%20pantalla%202024-08-29%20234231.png)
### 4. Configurar las Opciones de Autenticación

En la misma pestaña:

- **Tipo de autenticación**: Selecciona **"Clave SSH"** o **"Contraseña"**.
  - Si eliges **"Clave SSH"**, proporciona una clave SSH pública.
  - Si eliges **"Contraseña"**, establece un nombre de usuario y contraseña.

### 5. Configurar la Red

1. Navega a la pestaña **"Red"**.
2. Asegúrate de que la red virtual y la subred sean correctas.
3. Configura un **grupo de seguridad de red** (NSG) para permitir el tráfico entrante necesario (por ejemplo, permitir el puerto 22 para SSH).

![](/imgs/Captura%20de%20pantalla%202024-08-29%20234302.png)

### 6. Configuracion de disco

![](/imgs/Captura%20de%20pantalla%202024-08-29%20234253.png)

### 7. Revisar y Crear la Máquina Virtual

1. Haz clic en la pestaña **"Revisar + crear"**.
2. Revisa todas las configuraciones y asegúrate de que sean correctas.
3. Haz clic en **"Crear"** para comenzar el despliegue de la máquina virtual.

## Detener o Eliminar la Máquina Virtual

Para detener la VM:
1. Ve a la página de la VM en el portal de Azure.
2. Haz clic en **"Detener"**.

Para eliminar la VM:
1. Ve a la página de la VM en el portal de Azure.
2. Haz clic en **"Eliminar"**.

## Conclusión

Siguiendo estos pasos, podrás desplegar y gestionar una máquina virtual en Azure fácilmente a través del portal web. Este enfoque te permite crear rápidamente entornos de desarrollo, pruebas o producción de manera escalable y segura.

Evidencia de VM corriendo:

![](/imgs/vmrun.png)
![](/imgs/vm.png)