## Diseño 

## Use cases
-  acortar = tomamos el link original => retornamos una URL corta
- redireccionar = tomamos el link acortado y redireccionamos a la direccion URL orignal
- URL customizables


## Roadmap
- Analiticas
- Expiracion automatica
- Eliminacion manual
- UI vs API


## Calculo de recursos
- Nuevas URLs por mes: 100*10^6
- Request por mes: 1x10^9
- Request por segundo 400 donde son 40 nuevos acortadores y 360 redirecciones.
- URLs en 5 años: 6*10^9
- Bytes por URL: 500 bytes.
- Bytes por hash: 6bytes.
- Storage necesario por 5 años: 3TBs para todas las URLs, y 36Gbs por todos los hashes por 5 años.
- computo de escritura por segundo: 40 * (500 + 6) = 20kbs
- computo de lectura por segundo: 360 * 560 bytes = 190Kbs


## Diseño abstracto
- Capa de aplicacion donde tenemos los servicios de redireccion y acortamiento
- capa de persistencia de datos donde guardamos las url y hashes


## Cuellos de botella



## como escalar





