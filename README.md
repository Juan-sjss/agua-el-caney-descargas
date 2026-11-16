# Agua el Caney — Descargas

Repositorio público usado **solo para alojar los instaladores APK** de las dos
aplicaciones Android del proyecto Agua el Caney. No contiene código fuente.

| Aplicación | Archivo | Enlace |
|---|---|---|
| Cliente | `AguaElCaney-Cliente-2026-11-15.apk` | [Descargar](https://github.com/Juan-sjss/agua-el-caney-descargas/releases/download/v1.0.0/AguaElCaney-Cliente-2026-11-15.apk) |
| Repartidor | `AguaElCaney-Repartidor-2026-11-15-v2.apk` | [Descargar](https://github.com/Juan-sjss/agua-el-caney-descargas/releases/download/v1.0.1/AguaElCaney-Repartidor-2026-11-15-v2.apk) |

Página con códigos QR: <https://juan-sjss.github.io/agua-el-caney-descargas/>

> **Repartidor v2 (15/11/2026):** la hoja de ruta muestra **todos los pedidos
> pendientes**, sin filtrar por día, con la fecha de entrega de cada pedido.
> Reemplaza a la versión anterior del repartidor; se instala encima porque
> conserva la misma firma y sube `versionCode` a 2.

## Verificación

| Archivo | Tamaño | SHA-256 |
|---|---|---|
| `AguaElCaney-Cliente-2026-11-15.apk` | 81 155 771 bytes | `78763F3E350126998503083AC8BF72C25D694205F06F10B02C8D56A419DD69E0` |
| `AguaElCaney-Repartidor-2026-11-15-v2.apk` | 81 131 079 bytes | `604878B422A8E144AA972C878DDFC98457AFF003931BB66980A6253F7FF9D0A9` |
| `AguaElCaney-Repartidor-2026-11-15.apk` (v1, obsoleta) | 81 131 963 bytes | `1ED68738B773FC6EAC88F42743BA6E3EE42A270AA2CAA455F1AABCE40F8755A0` |

Las descargas responden `200` con `Content-Disposition: attachment;
filename=AguaElCaney-...apk`. Las tres APK se compilaron con Hermes (JavaScript
como bytecode) y R8 en release.

## Cómo instalar

1. Abrir el enlace desde un teléfono Android (o escanear el QR).
2. Permitir la instalación de aplicaciones desde esa fuente cuando el navegador lo pregunte.
3. Abrir el archivo `.apk` y tocar **Instalar**.

## API

Las apps consumen la API desplegada en <https://el-caney-api.onrender.com>.
El plan gratuito de Render suspende la instancia tras unos 15 minutos sin uso:
la primera petición puede tardar cerca de un minuto mientras el servicio despierta.
