# Codelabs de PAMN

## Descripción  
Repositorio creado para guardar varios de los codelabs probado por el alumno en código kotlin en Android Studio durante el curso de la asignatura *PAMN*.

<img width="650" height="341" alt="image" src="https://github.com/user-attachments/assets/040f00fe-a5a7-4020-ac7d-a4a022173a6e" />

## Ejercicios Android - AndroidManifest.xml

### 1. [GreetingCard](./GreetingCard)

Primer ejercicio realizado para familiarizarse con el entorno de Android Studio y la estructura básica de una aplicación Android.

**Aspectos destacados:**
- **Reglas de backup modernas**: Incluye `dataExtractionRules` y `fullBackupContent` para gestión avanzada de copias de seguridad
- **Namespace tools**: Declara `xmlns:tools` para herramientas de desarrollo
- **Configuración completa de seguridad**: Referencias a archivos XML específicos para políticas de extracción y backup de datos
- **Tema aplicado a dos niveles**: Tanto en `<application>` como en `<activity>` para mayor control

### 2. [BasicsCodelab](./BasicsCodelab)

**Aspectos destacados:**
- **`android:exported="true"`**: Obligatorio desde Android 12 para actividades con intent-filters
- **Intent-filter MAIN/LAUNCHER**: Define el punto de entrada de la app
- **`android:supportsRtl="true"`**: Soporte para idiomas RTL (derecha a izquierda)
- **Configuración estándar**: Backup habilitado, iconos redondos y tema personalizado

### 3. [CardViewKotlin](./CardViewKotlin)

**Aspectos destacados:**
- **`android:allowBackup="false"`**: Desactiva explícitamente el backup (útil para apps con datos sensibles)
- **Package declarado**: Usa el atributo `package` (estilo antiguo, ahora gestionado por Gradle)
- **Actividad personalizada**: `CardViewActivity` en lugar de `MainActivity`
- **Configuración minimalista**: Solo elementos esenciales sin configuraciones de seguridad adicionales

### 4. [AnimationsInterpolatorPlayground](./AnimationsInterpolatorPlayground)

**Aspectos destacados:**
- **Nombre de actividad con ruta completa**: Usa el package completo en `android:name` (no recomendado, pero funcional)
- **Sin `android:exported`**: Código anterior a Android 12
- **Soporte RTL activado**: Preparado para internacionalización
- **Estructura simplificada**: Manifest directo enfocado en funcionalidad básica

### 5. [SwipeRefreshMultipleViews](./SwipeRefreshMultipleViews)

**Aspectos destacados:**
- **Versioning antiguo**: Incluye `versionCode` y `versionName` en el manifest (ahora se gestiona desde Gradle)
- **Comentario sobre SDK**: Indica explícitamente que las versiones SDK se manejan en `build.gradle`
- **Sin configuraciones de seguridad**: Ejemplo de código legacy sin políticas modernas de backup
- **Package explícito**: Estilo de configuración de versiones anteriores de Android
