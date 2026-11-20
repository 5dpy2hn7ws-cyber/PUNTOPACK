# PuntoPack — versión web pública (Vercel)

## Publicar gratis

1. Descomprime este ZIP y sube los tres archivos de esta carpeta a un repositorio nuevo de GitHub (por ejemplo `puntopack-web`).
2. En https://vercel.com/new inicia sesión con GitHub, selecciona ese repositorio y pulsa **Deploy**.
3. Framework Preset: **Other**; Root Directory: `./`; no hay comando de compilación.
4. Vercel te dará una dirección `*.vercel.app` (nombre sujeto a disponibilidad).
5. Comprueba la búsqueda de localidades, filtros, mapa y acceso desde móvil.

## Integraciones y límites

- El mapa base usa Leaflet y OpenStreetMap. La búsqueda usa Nominatim y la consulta comunitaria usa Overpass; ambos son servicios públicos con límites de uso, no adecuados para alto tráfico sin infraestructura propia o proveedor contratado.
- Los puntos comunitarios son parciales, no son catálogos oficiales.
- El Geowidget de InPost requiere clave pública asociada al dominio final. Se puede introducir en la interfaz. No garantiza la integración de marcadores InPost con los demás transportistas.
- **Esta entrega es estática:** no incluye el servidor Python de desarrollo ni el endpoint `/api/inpost/points`. No colocar credenciales privadas en el HTML ni en GitHub.
- Para producción con API oficial será necesario desplegar un backend protegido y obtener permiso y credenciales.
- Los datos de Vinted Go, SEUR, Celeritas y GLS aún no están integrados oficialmente.

## Uso

Abre la URL pública. Busca un municipio español, acerca el mapa y pulsa «Buscar puntos comunitarios en esta zona». Para InPost usa «Abrir mapa oficial InPost» e introduce la clave autorizada.
