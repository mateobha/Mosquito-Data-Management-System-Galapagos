# Guía de Instalación — Mosquito Data Management System Galápagos

## Requisitos del sistema

| Requisito | Mínimo |
|-----------|--------|
| Sistema operativo | Windows 10 de 64 bits o superior |
| Espacio en disco | ~1 GB libre |
| Permisos | Administrador (para instalar en Archivos de programa) |

---

## 1. Descargar el instalador

Ve a la página oficial de Releases:

➡️ https://github.com/mateobha/Mosquito-Data-Management-System-Galapagos/releases/latest

Descarga el archivo `DMQ Ovitrampas Monitor.exe`.

> ⚠️ Descarga **únicamente** desde este repositorio oficial.

---

## 2. Verificar la integridad

Antes de ejecutar el instalador, verifica el hash SHA-256 publicado en la release.

**En PowerShell:**

```powershell
Get-FileHash "DMQ Ovitrampas Monitor.exe" -Algorithm SHA256
```

El valor debe coincidir **exactamente** con el `SHA-256` publicado en la release.
Si no coincide, no ejecutes el archivo y descárgalo nuevamente.

---

## 3. Instalar

1. Haz doble clic en `DMQ Ovitrampas Monitor.exe`.
2. Si aparece un aviso de **Windows SmartScreen**, haz clic en **"Más información"**
   y luego en **"Ejecutar de todas formas"** (es normal para aplicaciones sin firma
   de código de pago).
3. Acepta el aviso de UAC (Control de cuentas de usuario) si aparece.
4. Sigue el asistente de instalación para elegir el directorio y crear accesos
   directos en el escritorio.

---

## 4. Primer inicio

Al abrir la aplicación por primera vez:

- Ingresa con las credenciales iniciales:
  - **Usuario:** `admin`
  - **Contraseña:** `admin123`
- Cambia la contraseña en el primer inicio de sesión.

---

## Solución de problemas comunes

| Problema | Solución |
|----------|----------|
| El mapa o los gráficos no cargan | Reinicia la aplicación |
| El antivirus bloquea el instalador | Verifica el hash SHA-256 y agrega una excepción |
| Error al iniciar en Windows 10 | Asegúrate de tener las actualizaciones de Windows instaladas |

¿Otro problema? Escribe a **mateo.bha@outlook.com** o abre un
[Issue](https://github.com/mateobha/Mosquito-Data-Management-System-Galapagos/issues).
