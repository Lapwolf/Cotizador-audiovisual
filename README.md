# Cotizador audiovisual

App web para cotizar servicios de edición, fotografía, videografía y manejo de redes sociales. Es un solo archivo (`index.html`), sin instalación ni servidor.

## Qué hace

- Cotiza por pestañas: grabación y equipos, edición, fotografía y redes sociales.
- Soles o dólares, con tipo de cambio editable.
- Descuento, adelanto y saldo; contrato mensual con descuento para redes sociales.
- Paquetes prediseñados, condiciones frecuentes con un clic y logo propio.
- PDF para el cliente, mensaje para WhatsApp y acuerdo de servicio.
- PDF interno con costos, comisión de quien refiere y ganancia neta.
- Historial de cotizaciones con estado, vigencia, estadísticas y respaldo.

## Publicarlo con GitHub Pages

1. Crea un repositorio nuevo en GitHub (por ejemplo `cotizador`).
2. Sube `index.html` y este `README.md` (botón **Add file → Upload files**).
3. Ve a **Settings → Pages**.
4. En **Build and deployment**, elige **Deploy from a branch**, rama `main` y carpeta `/ (root)`.
5. Guarda. En uno o dos minutos la app queda en `https://TU-USUARIO.github.io/cotizador/`.

También puedes abrir `index.html` directo en el navegador, sin subirlo a ningún lado.

## Dónde se guardan los datos

Todo se guarda en el navegador (`localStorage`) del dispositivo donde lo uses. No se envía a ningún servidor.

- Cada navegador y cada dispositivo tiene su propio historial.
- Si borras los datos del navegador, se pierde el historial.
- Usa **Historial y respaldo → Copiar respaldo** para guardar una copia en texto, y **Restaurar desde texto** para recuperarla en otro dispositivo.

## Personalizar precios y servicios

Al inicio del bloque `<script>` de `index.html` está la lista `TABS`. Cada servicio es una línea con este formato:

```
["Categoría", "Nombre del servicio", "unidad", precio_en_soles]
```

Cambia los textos y precios, o agrega líneas nuevas **al final de cada pestaña** para no desordenar las cotizaciones ya guardadas.

Los precios actuales y los servicios de fotografía y redes sociales son ejemplos. Ajústalos a tus tarifas.

## Antes de usarlo con clientes

El texto del acuerdo de servicio y las condiciones frecuentes (derechos de uso, cancelación en 48 horas, rondas de cambios) son una base general. Revísalos y adáptalos a cómo trabajas.
