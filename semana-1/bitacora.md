# Bitácora de inspección HTTP - Joao

# Bitácora de inspección HTTP - Joao Sebastian Vargas

## 1. Sitio del Estado: DANE
- **URL:** https://www.dane.gov.co/
- **Fecha/Hora:** 07/05/2026 - 10:30 AM
- **Estado:** 200 OK
- **TTFB:** 297 ms
- **Tamaño total:** 2.8 MB
- **Total peticiones:** 190
- **Redirecciones:** 301 observada (HTTP a HTTPS)
- **Certificado:** Sectigo Limited (Expira: 03/08/2026)


---

## 2. Sitio Universitario: FUMC
- **URL:** https://www.fumc.edu.co/
- **Fecha/Hora:** 8/05/2026 - 10:48 AM
- **Estado:** 200 OK
- **TTFB:** 3.69 s
- **Tamaño total:** 1.5 MB
- **Total peticiones:** 207
- **Redirecciones:** Ninguna observada
- **Certificado:** GlobalSign nv-sa (Expira: 07/11/2026)


---

## 3. Sitio Comercial: Mercado Libre
- **URL:** https://www.mercadolibre.com.co/
- **Fecha/Hora:** 08/05/2026 - 10:55 AM
- **Estado:** 200 OK
- **TTFB:** 429 ms
- **Tamaño total:** 493 kB
- **Total peticiones:** 242
- **Redirecciones:** 301
- **Certificado:** Amazon (Expira: 15/11/2026)

https://github.com/joaosebastian1234-sudo/lenguajes-web-joaosebastianvargas-2026/blob/993b170000a89d642f139c35f3def791849a56d2/Mercado%20libre%20analisis.png

---

## 6. Reflexión Final (Análisis comparativo)

Tras la observación empírica de los tres sitios, se concluye que **Mercado Libre** es el más eficiente en términos de carga inicial, con un tamaño transferido de apenas 493 kB a pesar de realizar 242 peticiones. Esto se debe a una excelente optimización de recursos (imágenes webp y scripts minificados) y un **TTFB** significativamente bajo comparado con los sitios institucionales.

En cuanto a las **redirecciones**, tanto el DANE como Mercado Libre utilizan códigos **301** para forzar el uso de protocolos seguros, una práctica estándar de ciberseguridad. La FUMC mostró una carga directa, aunque con una cantidad elevada de peticiones (207) que elevan el tiempo final de renderizado a casi 8 segundos.

Finalmente, los **certificados TLS** varían según la organización: el Estado usa Sectigo, la Universidad usa GlobalSign y el sitio comercial usa Amazon. Esta diversidad demuestra que cada entidad elige su autoridad certificadora según su infraestructura (por ejemplo, Mercado Libre usa la de su proveedor de nube). La comparativa cuantitativa deja claro que el sector comercial prioriza la velocidad de respuesta para mejorar la experiencia de usuario, mientras que los sitios estatales e institucionales manejan cargas de archivos más pesadas que afectan el rendimiento.
