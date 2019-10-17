# API HYCPL - Procedencias/Leer

### Introducción

El catálogo de procedencias permite indicar la procedencia de los huéspedes en las reservaciones.

Se presentan dos endpoints. Una para obtener una lista general y otro para consultar un código de procedencia en particular.

### EndPoint Procedencias/Leer
```
http://wshycpl.puntaleonaonline.com/api/Procedencias/Leer?codigoProcedencia={codigo}
```

**Ejemplo**

- cURL


    curl -X POST \
      'http://wshycpl.puntaleonaonline.com/api/Procedencias/Leer?codigoProcedencia=188' \
      -H 'Accept: */*' \
      -H 'Accept-Encoding: gzip, deflate' \
      -H 'Authorization: Bearer KC63xfbVOCcHf0CZJhE_NbymexfYljMDOULHY6KGv-cnTH861eyAEkgAdjTbzyJsoylrSlT4rVS24wrTiVh1PAppJnqGKIsG9xoR5PgSl7zIP22r1o5ftz-hiqG1M-kBQ2eL72ad6EMAAKDj_PxsNsadCo88DG0r7uZUVzaugRyFuUR_EvA5UmVC-rW-N9NSMDfHVbSgGuKgqTvlzPfhBYmlpnthPvPXgDnWMBl55pe1Q_u14Qf9Ku4rqKm-VnYlRZunCgDW8h44oCP_fAJrHZ3YByNHYOuGd5FaHAInJg8RDpdoBjOndO_XeYFYUE8zFW6F9NmySOlJptSTZ4zh97Vndlz7nMaNQRvWEN_C0nF66zQbdQ4O6LvbCfYvDmDvCH6ArdF_AwlvmoKhgHWkoqb2w5lqXoVNRZuNb-P9ozGTiS0dwIgXqeyJxDPcx2KYiMBeUU4UQY7aBI-AgkQLaiKlZy-m-UIotEixh8G9cKNDPVC4KL10Qj6t41no-lYl' \
      -H 'Cache-Control: no-cache' \
      -H 'Connection: keep-alive' \
      -H 'Content-Length: 0' \
      -H 'Content-Type: application/json' \
      -H 'Host: wshycpl.puntaleonaonline.com' \
      -H 'Postman-Token: c3610d34-6943-4d7b-bf03-35cd4cc018d5,6a1342f3-76fb-483a-8850-c1933b46c28a' \
      -H 'User-Agent: PostmanRuntime/7.18.0' \
      -H 'cache-control: no-cache'


- **Respuesta esperada**


    {
        "codigoProcedencia": 188,
        "nombreProcedencia": "COSTA RICA"
    }



# Códigos de estado de respuesta HTTP

Cualquier estado distinto al 200, debe considerarse como un error de la solicitud.

- 404 Not Found  es un resultado si se indica un código de procedencia que no existe.

