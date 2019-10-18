# API Ministerio de Hacienda

# Introducción

Información general y de uso público para el consumo desde aplicaciones creadas por desarrolladores de soluciones.

# EndPoints
## https://api.hacienda.go.cr/fe/ae

Permite obtener el nombre, el tipo de identificación, el régimen y las actividades económicas asociadas a un contribuyente, usando como parámetro el número de identificación (sin hacer uso de guiones).  Para la consulta de identificaciones físicas nacionales no es necesario incluir el 0 como primer dígito. En el caso de las identificaciones jurídicas es necesario el uso de los primeros 10 dígitos, sin utilizar los dos últimos dígitos verificadores. Lo anterior, aplica del mismo modo para los Nites tributarios.

Identificaciones soportadas:

1. Físicas nacionales
2. Jurídicas nacionales
3. DIMEX
4. Nites tributarios

**Ejemplos**

- cURL


    curl --location --request GET "https://api.hacienda.go.cr/fe/ae?identificacion=2100042005"


- jQuery


    $.ajax({
      "url": "https://api.hacienda.go.cr/fe/ae?identificacion=2100042005",
      "method": "GET"
    }).done(function (response) {
      console.log(response);
    });


- PHP


    <?php
    
    $curl = curl_init();
    
    curl_setopt_array($curl, array(
      CURLOPT_URL => "https://api.hacienda.go.cr/fe/ae?identificacion=2100042005",
      CURLOPT_RETURNTRANSFER => true,
      CURLOPT_ENCODING => "",
      CURLOPT_MAXREDIRS => 10,
      CURLOPT_TIMEOUT => 0,
      CURLOPT_FOLLOWLOCATION => false,
      CURLOPT_HTTP_VERSION => CURL_HTTP_VERSION_1_1,
      CURLOPT_CUSTOMREQUEST => "GET",
    ));
    
    $response = curl_exec($curl);
    $err = curl_error($curl);
    
    curl_close($curl);
    
    if ($err) {
      echo "cURL Error #:" . $err;
    } else {
      echo $response;
    } ?>

**Respuesta esperada**


    {
      "nombre": "ESTADO-MINISTERIO DE HACIENDA",
      "tipoIdentificacion": "02",
      "regimen": {
        "codigo": 1,
        "descripcion": "Régimen Tradicional"
      },
      "actividades": [
        {
          "estado": "I",
          "codigo": 751101,
          "descripcion": "ACTIVIDADES DE LA ADMINISTRACION PUBLICA EN GENERAL"
        }
      ]
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

