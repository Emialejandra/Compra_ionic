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

## Evidencias 


