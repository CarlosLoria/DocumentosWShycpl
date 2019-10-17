# API HYCPL - DatosAcciones/Actualizar

### Introducción

DatosAcciones/Actualizar permite actualizar datos de una Acción.  

### EndPoint
```
http://wshycpl.puntaleonaonline.com/api/DatosAcciones/Actualizar
```

Permite actualizar datos de la acción referenciada.

**Campos por actualizar**

- Solamente se actualizan los campos asignados.  Por ejemplo si "telefonoOficina" viene en blanco, es decir "", dicho campo no se actualiza en la base de datos de socios.

**Ejemplo**

- cURL


    curl -X POST \
      http://wshycpl.puntaleonaonline.com/api/DatosAcciones/Actualizar \
      -H 'Accept: */*' \
      -H 'Accept-Encoding: gzip, deflate' \
      -H 'Authorization: Bearer MSD1KkjXQ22MqBH_DViXTxShg13YadjweGZpHaJgd-BE0Y-uqZZKjvFSXLURnmJrCgEqcJTv89H5xb7KH2xJIWhGY8anNoWyrbDgVyD6kh0BpHVmf5fCUgnq8ofoIy73n4nlnt09X6QGS95JND-_384ueBk-SJaWBdCKOHJ277TBNgRuBGW6nH8T3Tt_ao5sHejfxX_MZURLyc6dkRBstqOD34qOWCdhpNGi9YYtP-_rOA35ElaTRV8y3iLglbYBu2kOohAgwE09yaApO8AtHFzUvq5Lkmtm4X_nKIeqoLi5xNGjSwBfrc0S19oSWyWSs7_oMZDs59EESkXERjIWHchl3BIBySAZVOD1y7HdfmBXK-9AIU1oa4-pL7a553UC-SMeCpHrPprNLC1aloAntU-1JbCfoIJI6nT8E4eTL9WzFIdi32xJXssr9arJWVUwgXqVLNRuclAhYS7twwANbMHcgzcsV_80oOmuy9nP1TEy2GWQqq4wWy6kPmhLXe6d' \
      -H 'Cache-Control: no-cache' \
      -H 'Connection: keep-alive' \
      -H 'Content-Length: 344' \
      -H 'Content-Type: application/json' \
      -H 'Host: wshycpl.puntaleonaonline.com' \
      -H 'Postman-Token: 54f539ef-7d5b-42f4-a1c9-4265910f6708,eec515de-0bb3-4670-b001-cc9b2b3baa29' \
      -H 'User-Agent: PostmanRuntime/7.18.0' \
      -H 'cache-control: no-cache' \
      -d '{
        "codigoAccion": 3,
        "telefonoCasa": "2232-6646",
        "telefonoOficina": "",
        "telefonoCelular": "",
        "telefonoFax": "",
        "telefonoOtro": "",
        "DireccionCobro": "DEL BALCON VERDE 3 CUADRAS N-O 75MTS N MANO IZQ PORTON CAFE CLARO",
        "DireccionCasa": "",
        "email": "f.salasl1939@gmail.com",
        "email2": "",
    }'


- **Respuesta esperada**


    {
        "DatosAccionID": 15,
        "FechaActualiza": "2019-10-17T07:21:21.4476105-06:00",
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
    }



- **En la respuesta, se muestran campos adicionales:**		

  ```
  Se muestra identificación asignada por la base de datos en DatosAccionID. También se muestra la fecha y hora en que se recibe la actualizacion en "FechaActualiza".
  ```

  

# Códigos de estado de respuesta HTTP

- Cualquier estado distinto al 200 debe ser considerado como un error en la solicitud.

  ```
  404 "Not found" - Si no existiera la acción referenciada.
  400 "Bad request" - cuando el falta algún dato requerido o se excede el máximo permitido.
  ```

  