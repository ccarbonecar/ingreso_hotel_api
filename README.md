# Enunciado

Se debe diseñar e implementar un api rest que devuelva las reservas de vuelo y los hoteles disponibles para un destino que se envía por parámetro. No es necesario que esta api esta securizada pero es un plus.

Las reservas de vuelo se obtienen de un sistema externo y tienen una duración de 10 minutos desde el momento de la consulta, pasado dicho tiempo es necesario volver a consultar el sistema puesto que las reservas se borran del sistema de consultas de reservas.

Se debe asumir que la api de reservas existe, no es necesario desarrollarla, es suficiente con un mock.

Para los hoteles del destino se puede usar la API:

```
https://api.foursquare.com/v2/venues/search?near={param1}&intent={param2}&query={param3}&client_id={param4}&client_secret={param5}&v={param6}

```

Para eso va a ser necesario crear una cuenta en:
https://foursquare.com/developers/login?continue=%2Fdevelopers%2Fapps

Para más documentación:
https://location.foursquare.com/developer/reference/api-overview

Un ejemplo de la llamada seria:

```
curl 'https://api.foursquare.com/v2/venues/search?near=roma&intent=browse&query=hotel&client_id={param4}&client_secret={param5}&v=20190709'

```

Se adjunta un ejemplo de la respuesta en el archivo "hoteles_respuesta.json"

# Criterios de evaluación

La api deberá ser implementada con sprintboot y java. Se pueden utilizar todos los frameworks, bases de datos, dockerfile y cualquier cosa que se considere necesaria.

El enunciado es abierto y se pueden asumir todo tipo de hipótesis a fines de simplificar el desarrollo o bien extenderlo para ser mas extenso en el uso de las tecnologías.

Se tendrá en consideración la calidad del código, test y arquitectura seleccionada para la implementacion, justificación y documentación de la misma.
