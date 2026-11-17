# Agua el Caney — Descargas

Repositorio público usado **solo para alojar los instaladores APK** de las dos
aplicaciones Android del proyecto Agua el Caney. No contiene código fuente.

| Aplicación | Archivo | Enlace |
|---|---|---|
| Cliente | `AguaElCaney-Cliente-2026-11-16.apk` | [Descargar](https://github.com/Juan-sjss/agua-el-caney-descargas/releases/download/v1.1.0/AguaElCaney-Cliente-2026-11-16.apk) |
| Repartidor | `AguaElCaney-Repartidor-2026-11-16.apk` | [Descargar](https://github.com/Juan-sjss/agua-el-caney-descargas/releases/download/v1.1.0/AguaElCaney-Repartidor-2026-11-16.apk) |

Página con códigos QR: <https://juan-sjss.github.io/agua-el-caney-descargas/>

> **Release v1.1.0 (16/11/2026):** iconos de la marca. El cliente estrena el
> logo de Agua el Caney (`versionCode` 2) y el repartidor la moto con el nombre
> “Agua el Caney” en rojo (`versionCode` 3). Se instalan encima de las versiones
> anteriores porque conservan la misma firma, así que no hay que desinstalar.
> El repartidor mantiene la hoja de ruta con **todos los pedidos pendientes** y
> la fecha de cada uno (cambio publicado en `v1.0.1`).

## Verificación

| Archivo | Tamaño | SHA-256 |
|---|---|---|
| `AguaElCaney-Cliente-2026-11-16.apk` | 81 205 067 bytes | `F87C891D29696918368C1BC1D8D1122BF624C354ABE2EB9E0A3478E2E1C16BE3` |
| `AguaElCaney-Repartidor-2026-11-16.apk` | 81 014 239 bytes | `A1C27A84F0C95ED71C2FFC3C23DCA3A829B1F68FFFD2D26348485B19A9550350` |
| `AguaElCaney-Cliente-2026-11-15.apk` (v1, obsoleta) | 81 155 771 bytes | `78763F3E350126998503083AC8BF72C25D694205F06F10B02C8D56A419DD69E0` |
| `AguaElCaney-Repartidor-2026-11-15-v2.apk` (obsoleta) | 81 131 079 bytes | `604878B422A8E144AA972C878DDFC98457AFF003931BB66980A6253F7FF9D0A9` |

Las descargas responden `200` con `Content-Disposition: attachment;
filename=AguaElCaney-...apk`. Las APK se compilan con Hermes (JavaScript
como bytecode) y R8 en release.

## Cómo instalar

1. Abrir el enlace desde un teléfono Android (o escanear el QR).
2. Permitir la instalación de aplicaciones desde esa fuente cuando el navegador lo pregunte.
3. Abrir el archivo `.apk` y tocar **Instalar**.

## API

Las apps consumen la API desplegada en <https://el-caney-api.onrender.com>.
El plan gratuito de Render suspende la instancia tras unos 15 minutos sin uso:
la primera petición puede tardar cerca de un minuto mientras el servicio despierta.
