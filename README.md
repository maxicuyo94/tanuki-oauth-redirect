# Tanuki — retorno de Mercado Libre

Página estática para recibir el código de autorización OAuth de Mercado Libre y
mostrar la URL de retorno que se pega en Tanuki. No contiene credenciales, no
envía el código a ningún servicio adicional y borra los parámetros de la barra
de direcciones después de cargarlos en memoria.

Sitio público: https://maxicuyo94.github.io/tanuki-oauth-redirect/

El código de autorización se intercambia por tokens únicamente en Tanuki. La
aplicación usa PKCE y comprueba el parámetro `state` antes del intercambio.
