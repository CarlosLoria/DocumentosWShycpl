# API HYCPL - DatosAcciones

# Introducción

DatosAcciones permite actualizar datos de una Accion

# EndPoint
## http://wshycpl.puntaleonaonline.com/api/DatosAcciones/Actualizar

Permite actualizar datos de la accion referenciada.


**Ejemplos**

curl -X POST \
  http://localhost:14960/api/DatosAcciones/Actualizar \
  -H 'Accept: */*' \
  -H 'Accept-Encoding: gzip, deflate' \
  -H 'Authorization: Bearer IDRnFDifha7F9ksh1BdNTB5_2eROq5y0nDEAA9_pINYK4MVtRYGGhep7nZxN74bI91NEhnQ7rN2l6_s_WuvgGab4tRI40l65SvUFB-HvJn0VhXWW4gRBqqBW5FvlwvheO7CLvg0QoxC6SW9HE-aDkEEoaCoadcNg3jgY56m71rCdI-nnz-oMYoJtuUw5ttVQs6jRn7ZItCQ_R3CQmAQWvNsv78qgkdhpJnGhH7glFu9OAqDKRtUGqS3HT0NecC8M_lq-JHtRvaf9av0cC6Ql-yI7Glm36YvjXZhOXLHGZQVV0weBV9kGVkQJaiMD7Bxp9s6SRrfSr0xy5jn_ttod-kdF09KQfI6JE97QpTkbhIyTJPoCR0MAW1svxNPLz4Ll9mRf4mmg0n4uuOD7SH5dLWusnsaN91iBkHzhl6bHSx0CuGW0swidh2_h4WDZO0rn1kuKu80I5R2rX9LrrUjeGGYGY8GJ7ideWrNliZO2hd_Txbgv4894_-WHoNBTdQ2V' \
  -H 'Cache-Control: no-cache' \
  -H 'Connection: keep-alive' \
  -H 'Content-Length: 380' \
  -H 'Content-Type: application/json' \
  -H 'Host: localhost:14960' \
  -H 'Postman-Token: 7a2d6508-096b-4a7e-84b0-a37293ad9644,5e96efdd-46b0-40e8-b06e-15376dd3ecd4' \
  -H 'User-Agent: PostmanRuntime/7.18.0' \
  -H 'cache-control: no-cache' \
  -d '{
  "FechaActualiza": "2019-10-16T06:27:50.7072678-06:00",
  "codigoAccion": 3,
  "telefonoCasa": "22326646",
  "telefonoOficina": "",
  "telefonoCelular": "",
  "telefonoFax": "",
  "telefonoOtro": "",
  "DireccionCobro": "DEL BALCON VERDE 3 CUADRAS N-O 75MTS N MANO IZQ PORTON CAFE CLARO",
  "DireccionCasa": "",
  "email": "f.salasl1939@gmail.com",
  "email2": ""
}'

**Respuesta esperada**
{
    "DatosAccionID": 3,
    "FechaActualiza": "2019-10-16T06:27:50.7072678-06:00",
    "codigoAccion": 3,
    "telefonoCasa": "22326646",
    "telefonoOficina": "",
    "telefonoCelular": "",
    "telefonoFax": "",
    "telefonoOtro": "",
    "DireccionCobro": "DEL BALCON VERDE 3 CUADRAS N-O 75MTS N MANO IZQ PORTON CAFE CLARO",
    "DireccionCasa": "",
    "email": "f.salasl1939@gmail.com",
    "email2": ""
}


**Tipos de identificación**

- 01 Persona física costarricense
- 02 Persona jurídica costarricense estatal (pública) o persona jurídica costarricense privada
- 03 Persona física extranjera (DIMEX)
- 04 Número de identificación tributario para personas físicas (NITE)

**Tipos de regímenes**

- 0 No tiene 
- 1 Régimen tradicional
- 2 Régimen simplificado


## https://api.hacienda.go.cr/indicadores/tc/dolar

Permite obtener el tipo de cambio del dólar de los Estados Unidos de América.  No requiere de ningún tipo de parámetro.

**Ejemplos**

- cURL


    curl --location --request GET "https://api.hacienda.go.cr/indicadores/tc/dolar"


- jQuery


    $.ajax({
      "url": "https://api.hacienda.go.cr/indicadores/tc/dolar",
      "method": "GET"
    }).done(function (response) {
      console.log(response);
    });

**Respuesta esperada**


    {
      "venta": {
        "fecha": "2019-07-24T00:00:00-06:00",
        "valor": "575.97"
      },
      "compra": {
        "fecha": "2019-07-24T00:00:00-06:00",
        "valor": "570.44"
      }
    }


# Códigos de estado de respuesta HTTP

Cualquier estado distinto al 200, puede considerarse como un error de la solicitud:

- 404 cuando una identificación no aparece registrada
- 400 cuando el número de identificación enviado en el request es considerado como un dato no válido.

