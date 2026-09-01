# Guía de Publicación de la Web App de iOS en GitHub Pages

Este proyecto contiene la Progressive Web App (PWA) de la Credencial Digital adaptada especialmente para dispositivos iOS (iPhone y iPad).

Para publicarla de manera remota en su repositorio exclusivo, sigue estos pasos desde la consola de tu ordenador:

---

## Paso 1: Abrir la terminal en esta carpeta
Abre PowerShell o tu consola favorita y colócate en esta carpeta específica:
```powershell
cd "C:\Users\Jonathan\Desktop\Papá academia\Antigravity Proyects\Gestion_de_credenciales_Andorid_IOS\Web App para IOS"
```

---

## Paso 2: Inicializar Git y vincular el repositorio oficial

Ejecuta la siguiente secuencia de comandos para inicializar Git a nivel local dentro de esta carpeta (manteniéndola totalmente independiente de la aplicación principal):

```powershell
# Inicializar Git en esta carpeta independiente
git init

# Agregar los archivos (index.html, manifest.json, logo.png, etc.)
git add .

# Hacer el commit de la primera versión
git commit -m "Publicacion inicial de la Web App para iOS"

# Cambiar la rama por defecto a main
git branch -M main

# Vincular con el repositorio exclusivo de la Web App
git remote add origin https://github.com/Sindicarnecolon/credenciales-ios-webapp.git
```

---

## Paso 3: Subir los archivos a GitHub

Si tienes la sesión iniciada correctamente en GitHub con la cuenta `Sindicarnecolon`, ejecuta:
```powershell
git push -u origin main
```

*(Si es necesario, el sistema te solicitará autorización en tu navegador para realizar la carga)*.

---

## Paso 4: Activar GitHub Pages

1. Abre tu navegador y dirígete al repositorio en GitHub:
   [https://github.com/Sindicarnecolon/credenciales-ios-webapp](https://github.com/Sindicarnecolon/credenciales-ios-webapp)
2. Ve a la pestaña **Settings** (Configuración) en la barra superior del repositorio.
3. En la barra lateral izquierda, haz clic en **Pages**.
4. En la sección **Build and deployment**:
   * **Source**: Asegúrate de que diga **Deploy from a branch**.
   * **Branch**: Selecciona **`main`** y la carpeta **`/(root)`** (ya que los archivos están en la raíz del repositorio).
5. Haz clic en **Save** (Guardar).

Una vez que se complete la compilación en GitHub (aproximadamente 1 minuto), el sitio estará en línea en la URL oficial:
**`https://sindicarnecolon.github.io/credenciales-ios-webapp/`**

---

## 📱 Cómo lo utiliza el usuario final en su iPhone/iPad:
1. Abre **Safari** (o cualquier navegador moderno) y accede a `https://sindicarnecolon.github.io/credenciales-ios-webapp/`.
2. Inicia sesión con su **DNI** y **Nombre y Apellido**.
3. Accede directamente a su **Credencial Digital**, generación de **Código QR**, **Novedades** y **Configuración**.
4. Para tener acceso rápido como app nativa, puede pulsar **Compartir** en Safari y seleccionar **"Añadir a pantalla de inicio"**.
