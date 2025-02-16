# React Native App - Autos

Este repositorio contiene una aplicación móvil desarrollada con **React Native** y **Expo**, creada utilizando la plantilla en blanco de Expo. La aplicación se centra en la gestión y visualización de autos.

## Requisitos previos

Asegúrate de tener instaladas las siguientes herramientas en tu máquina:

- Node.js (v14 o superior)
- npm (v6 o superior)
- Expo CLI (`npm install -g expo-cli`)
- EAS CLI (`npm install -g eas-cli`)

## Instalación

Sigue los siguientes pasos para clonar y ejecutar la aplicación localmente:

1. Clona el repositorio:

   ```bash
   git clone https://github.com/AntonySP22/autos
   cd autos
   ```

2. Instala las dependencias utilizando Expo:

   ```bash
   npx create-expo-app@latest autos --template blank
   ```

3. Instala las dependencias adicionales:

   ```bash
   npx expo install react-dom react-native-web @expo/metro-runtime
   ```

## Desarrollo

Para iniciar el proyecto en modo de desarrollo, ejecuta el siguiente comando:

```bash
npx expo start
```

Esto abrirá Expo Developer Tools en tu navegador web. Desde allí, podrás escanear el código QR con la aplicación Expo Go para ver la aplicación en tu dispositivo o ejecutarla en un emulador.

## Linter y Formateo

Se configuró **ESLint** y **Prettier** para garantizar un código consistente y limpio.

1. Instalar las configuraciones de linting y formateo:

   ```bash
   npx expo install prettier eslint-config-prettier eslint-plugin-prettier --save-dev
   ```

2. Ejecutar el linter:

   ```bash
   npx expo lint
   ```

## Construcción y despliegue

Esta aplicación utiliza **EAS** para la construcción de versiones de producción.

1. Inicia sesión en EAS:

   ```bash
   eas login
   ```

2. Configura EAS para tu proyecto:

   ```bash
   eas build:configure
   ```

3. Construye la aplicación para Android:

   ```bash
   eas build -p android --profile production
   ```

Sigue las instrucciones proporcionadas por EAS para descargar e instalar el APK generado.
