# Lab09 - Consumo de API con Retrofit

## Instrucciones para abrir en Android Studio

1. **Abre Android Studio**
2. Selecciona **"Open"** (no "New Project")
3. Navega hasta la carpeta `Lab09` y selecciónala
4. Espera que Gradle sincronice (puede tardar 1-2 minutos)
5. Si pide actualizar el AGP (Android Gradle Plugin), acéptalo
6. Ejecuta en emulador o dispositivo físico

## Si hay errores de Gradle

- Ve a **File > Invalidate Caches > Invalidate and Restart**
- O borra la carpeta `.gradle` y vuelve a abrir

## Estructura del proyecto

```
com.example.lab09/
├── MainActivity.kt       → Scaffold, navegación, Retrofit init
├── PostModel.kt          → Data class del JSON
├── PostApiService.kt     → Interface con endpoints GET
├── moduloPosts.kt        → ScreenPosts y ScreenPost (UI)
└── ui/theme/
    └── Theme.kt          → Tema Material 3
```

## API usada

- **URL base:** `https://jsonplaceholder.typicode.com/`
- **Endpoints:**
  - `GET /posts` → Lista de posts
  - `GET /posts/{id}` → Post por ID

## Notas
- El permiso de INTERNET ya está en AndroidManifest.xml
- Todas las dependencias ya están en build.gradle.kts
