# API HYCPL - DatosAcciones/Consulta

### Introducción

DatosAcciones/Consulta  permite consultar los registros de actualizaciones recibidas para una acción.  

### EndPoint
```
http://wshycpl.puntaleonaonline.com/api/DatosAcciones/Consulta?codigoAccion={codigo}
```

Permite actualizar datos de la acción referenciada.

**Muestra actualizaciones que se han registrado para la acción consultada **

- Solamente se actualizan los campos asignados.  Por ejemplo si "telefonoOficina" biene en blanco, es decir "", dicho campo no se actualiza en la base de datos de socios.

**Ejemplo**

- cURL


    curl -X POST \
      'http://wshycpl.puntaleonaonline.com/api/DatosAcciones/Consulta?codigoAccion=3' \
      -H 'Accept: */*' \
      -H 'Accept-Encoding: gzip, deflate' \
      -H 'Authorization: Bearer KC63xfbVOCcHf0CZJhE_NbymexfYljMDOULHY6KGv-cnTH861eyAEkgAdjTbzyJsoylrSlT4rVS24wrTiVh1PAppJnqGKIsG9xoR5PgSl7zIP22r1o5ftz-hiqG1M-kBQ2eL72ad6EMAAKDj_PxsNsadCo88DG0r7uZUVzaugRyFuUR_EvA5UmVC-rW-N9NSMDfHVbSgGuKgqTvlzPfhBYmlpnthPvPXgDnWMBl55pe1Q_u14Qf9Ku4rqKm-VnYlRZunCgDW8h44oCP_fAJrHZ3YByNHYOuGd5FaHAInJg8RDpdoBjOndO_XeYFYUE8zFW6F9NmySOlJptSTZ4zh97Vndlz7nMaNQRvWEN_C0nF66zQbdQ4O6LvbCfYvDmDvCH6ArdF_AwlvmoKhgHWkoqb2w5lqXoVNRZuNb-P9ozGTiS0dwIgXqeyJxDPcx2KYiMBeUU4UQY7aBI-AgkQLaiKlZy-m-UIotEixh8G9cKNDPVC4KL10Qj6t41no-lYl' \
      -H 'Cache-Control: no-cache' \
      -H 'Connection: keep-alive' \
      -H 'Content-Length: 0' \
      -H 'Content-Type: application/json' \
      -H 'Host: wshycpl.puntaleonaonline.com' \
      -H 'Postman-Token: 10843fc2-30a1-48a0-ab7d-dd88e6d8a374,320d267d-f695-4a29-a94e-7edb97c8cd73' \
      -H 'User-Agent: PostmanRuntime/7.18.0' \
      -H 'cache-control: no-cache'


- **Respuesta esperada**


    [
        {
            "DatosAccionID": 15,
            "FechaActualiza": "2019-10-17T07:21:21.447",
            "codigoAccion": 3,
            "telefonoCasa": "2232-6646",
            "telefonoOficina": "",
            "telefonoCelular": "",
            "telefonoFax": "",
            "telefonoOtro": "",
            "DireccionCobro": "DEL BALCON VERDE 3 CUADRAS N-O 75MTS N MANO IZQ PORTON CAFE CLARO",
            "DireccionCasa": "",
            "email": "f.salasl1939@gmail.com",
            "email2": ""
        },
        {
            "DatosAccionID": 16,
            "FechaActualiza": "2019-10-17T07:38:27.767",
            "codigoAccion": 3,
            "telefonoCasa": "22326646",
            "telefonoOficina": "",
            "telefonoCelular": "",
            "telefonoFax": "",
            "telefonoOtro": "",
            "DireccionCobro": "",
            "DireccionCasa": "",
            "email": "",
            "email2": ""
        }
    ]



# Códigos de estado de respuesta HTTP

Cualquier estado distinto al 200, debe considerarse como un error de la solicitud.

