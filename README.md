# Compra

Aplicación móvil para registrar una compra y calcular el pago correspondiente. Está construida con Ionic y Angular, y preparada para ejecutarse en Android mediante Capacitor.

## Funcionalidades

- **Inicio:** presenta la aplicación y permite comenzar el flujo de compra.
- **Registro de compra:** captura el nombre del producto, la cantidad y el precio unitario. Valida que los campos estén completos, que la cantidad sea un entero positivo y que el precio sea mayor que cero.
- **Resumen y pago:** muestra los datos registrados y el subtotal. Permite ingresar un descuento entre 0 % y 100 % y el dinero recibido, y calcula el total final.
- **Resultado:** muestra el descuento aplicado y el cambio cuando el pago alcanza el total, o el saldo pendiente cuando falta dinero.
- **Navegación por pestañas:** organiza las vistas de inicio, registro de compra y pago.

Los datos de la compra se comparten entre las pantallas mediante un servicio de Angular en memoria. Al reiniciar la aplicación, la compra registrada no se conserva.

## Tecnologías

- Angular 
- Ionic Angular 
- Capacitor 
- TypeScript y SCSS

## Requisitos

- Node.js y npm
- Android Studio y Android SDK para compilar o ejecutar la versión Android

## Instalación y ejecución

Instala las dependencias desde la carpeta del proyecto:

```bash
npm install
```

Inicia la aplicación en el navegador:

```bash
ionic serve
```

El servidor de desarrollo de Angular mostrará en la terminal la dirección local para abrir la aplicación.

## Compilación para Android

Genera la versión web y sincronízala con el proyecto nativo de Android:

```bash
ionic build
ionic capacitor sync android
```

Para abrir el proyecto Android en Android Studio:

```bash
ionic capacitor open android
```

## Estructura principal

```text
src/app/
├── tab3/       # Pantalla de inicio
├── tab1/       # Registro y validación de la compra
├── tab2/       # Resumen, cálculo del pago y resultado
├── services/   # Datos compartidos de la compra
└── tabs/       # Navegación principal por pestañas
android/        # Proyecto nativo Android de Capacitor
resources/      # Recursos de la aplicación
```

# Evidencias

## 1. Ícono de la aplicación

<p align="center">
  <img src="https://github.com/user-attachments/assets/eca1652e-d44d-430c-888a-477ada60d678" width="280" alt="Ícono de la aplicación Compra">
</p>

## 2. Splash screen

<p align="center">
  <img src="https://github.com/user-attachments/assets/1f84286e-10e7-4d8b-9cad-9f6321e13975" width="250" alt="Pantalla de carga de la aplicación">
</p>

## 3. Pantalla de inicio

<p align="center">
  <img src="https://github.com/user-attachments/assets/32a2abec-91b1-449c-a9d5-fd7cf5ac3d8d" width="250" alt="Pantalla de inicio">
</p>

## 4. Registro de compra

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/901cb9fc-2b70-44db-87ce-a8b3635cd2ff" width="220" alt="Registro de compra">
      <br>
      <sub>Formulario de registro</sub>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/bdf99d43-e5e0-457c-8d24-45b7f35fb714" width="220" alt="Validación del formulario">
      <br>
      <sub>Validación de datos</sub>
    </td>
  </tr>
  <tr>
    <td align="center" colspan="2">
      <img src="https://github.com/user-attachments/assets/6b1fde77-d8a7-401e-ae3e-418629184d9e" width="220" alt="Registro de compra completado">
      <br>
      <sub>Registro de compra completado</sub>
    </td>
  </tr>
</table>

## 5. Resumen y pago de compra

<table>
  <tr>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/08f4375d-1e97-4208-8d60-1c8fa41eee53" width="220" alt="Resumen de compra">
      <br>
      <sub>Resumen y subtotal</sub>
    </td>
    <td align="center">
      <img src="https://github.com/user-attachments/assets/b50f331d-b258-4c17-828d-86d0a416e67c" width="220" alt="Cálculo del pago">
      <br>
      <sub>Descuento y pago</sub>
    </td>
  </tr>
  <tr>
    <td align="center" colspan="2">
      <img src="https://github.com/user-attachments/assets/0a1dbd34-87dc-4dfd-8e97-985207766fad" width="220" alt="Resultado del pago">
      <br>
      <sub>Resultado de la compra</sub>
    </td>
  </tr>
</table>
