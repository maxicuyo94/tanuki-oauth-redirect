# Tanuki — retorno de Mercado Libre

Página estática para recibir el código de autorización OAuth de Mercado Libre y
mostrar la URL de retorno que se pega en Tanuki. No contiene credenciales, no
envía el código a ningún servicio adicional y borra los parámetros de la barra
de direcciones después de cargarlos en memoria.

Sitio público: https://maxicuyo94.github.io/tanuki-oauth-redirect/

El código de autorización se intercambia por tokens únicamente en Tanuki. La
aplicación usa PKCE y comprueba el parámetro `state` antes del intercambio.

## Diseño

Usa los colores del sistema de diseño de Tanuki (`taller-admin`, `docs/sistema-de-diseno.md`; referencia completa en el artifact [Sistema Fukuro · Tanuki · PF](https://claude.ai/artifact/Dd8bZ2j7RvP49Hqa1G9Re2)), como variables CSS al principio de `index.html`. Sigue el tema claro u oscuro del navegador (`prefers-color-scheme`). Si cambian los colores de Tanuki, actualizá esas variables y medí el contraste en los dos temas (4,5:1 para texto).
