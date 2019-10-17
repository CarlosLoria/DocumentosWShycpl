# API HYCPL - Procedencias/Lista

### Introducción

El catálogo de procedencias permite indicar la procedencia de los huéspedes en las reservaciones.

Se presentan dos endpoints. Una para obtener una lista general y otro para consultar un código de procedencia en particular.

### EndPoint Procedencias/Lista
```
http://wshycpl.puntaleonaonline.com/api/Procedencias/Lista
```

**Ejemplo**

- cURL


    curl -X POST \
      http://wshycpl.puntaleonaonline.com/api/Procedencias/Lista \
      -H 'Accept: */*' \
      -H 'Accept-Encoding: gzip, deflate' \
      -H 'Authorization: Bearer l7LuyKcNGoKeaUw10dLTBU84Iq3HoK2Iy9XYD8Son8thUo9sHkJ9etJa3LQw4qGYz2ykw4r-rNCVJL0Vj8EAJ4jqDyWZ3iOl-DhYQj0w6QL1oW0C0LmGvuobuiyCk8vm7xSxOz1Js8xk6DNhylv1mOJKjPWKu05SpYCOrDcssCRbUxAPMXRdg0Q1AD87DHuvVE9TUwkVrW1uODCsD_gP3SKDP0u-yno8qRHK329-XoCtsxc7Qsv--03KUpOm55NRJL-LDuCUOCy284747kadQMaqpumZGTeJOaTO69cP9a_S2u-U757qeVeUmu1ffGMhCCUvbgWWcAgPhQ-XazUNHpot-EA9ktNLjw9SsOxomzFAzRoOKZMj4JUTOk07FBiwplkASFq6rZlyKvAVMYOax8KgqfbS9STRbduCm5hC51F-3Qf5iKUw7T__rw-8ILDOX1olqmDjDA2pHLc5oYVv09faDE6D92oh-ZHmIKUb8VmPEfbEQNb8rC27v-IrMLg3' \
      -H 'Cache-Control: no-cache' \
      -H 'Connection: keep-alive' \
      -H 'Content-Length: 0' \
      -H 'Content-Type: application/json' \
      -H 'Host: wshycpl.puntaleonaonline.com' \
      -H 'Postman-Token: 9da9e017-d591-4454-a499-2b1269888ca4,9c11281a-316f-4419-a691-b1de543a9fc3' \
      -H 'User-Agent: PostmanRuntime/7.18.0' \
      -H 'cache-control: no-cache'


- **Respuesta esperada**


    [
        {
            "codigoProcedencia": 4,
            "nombreProcedencia": "AFGHANISTAN"
        },
        {
            "codigoProcedencia": 8,
            "nombreProcedencia": "ALBANIA"
        }...
    
    	{
            "codigoProcedencia": 188,
            "nombreProcedencia": "COSTA RICA"
        },
        {
            "codigoProcedencia": 191,
            "nombreProcedencia": "CROATIA (local name: Hrvatska)"
        },
    	.
    	.
    	{
            "codigoProcedencia": 840,
            "nombreProcedencia": "ESTADOS UNIDOS DE AMERICA"
        },
        {
            "codigoProcedencia": 894,
            "nombreProcedencia": "ZAMBIA"
        }
    ]



# Códigos de estado de respuesta HTTP

Cualquier estado distinto al 200, debe considerarse como un error de la solicitud.

