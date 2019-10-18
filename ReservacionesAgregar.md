# API HYCPL - Reservaciones/Agregar

### Introducción

Para agregar una reservación es necesario incluir un registro con los datos de la misma indicando mediante un arreglo los tipos de habitaciones de la misma.

### EndPoint
```
http://wshycpl.puntaleonaonline.com/api/Reservaciones/Agregar
```

Permite actualizar datos de la acción referenciada.

**Ejemplo con dos tipos de habitación**

- Con este ejemplo de registro se agrega la reservación al sistema de reservaciones de Aristóteles. Para el nombre indicado, es decir “Carlos Loria”, una reservación del 22 al 27 de diciembre. En el ejemplo tiene dos tipos de habitación, una Selvamar y una Selvamar Superior King con Balcon. La Selvamar es en ocupación doble con un niño.  

  Por favor notar que el calculo total por cobrar debe venir incluido en el campo MontoTotal. Para esto debe de contemplarse la consulta de tarifa diaria para los periodos indicados.

  El código de agencia, por ahora sería “DIRECTA”, o eventualmente podríamos cambiarlo por un código de agencia que referencie el portal

**Ejemplo**

- cURL


    curl -X POST \
      http://wshycpl.puntaleonaonline.com/api/Reservaciones/Agregar \
      -H 'Accept: */*' \
      -H 'Accept-Encoding: gzip, deflate' \
      -H 'Authorization: Bearer V7QkuF1pHLmIb7b46cMFlk0NpnKlYGgaEaMeVokkyzVcobtCChN18h8RvNkEm3XfSySl5pxMj1mx2zTV4o9P3M1rz4YoUGa0PnIN0iT4tIar4vAs0_56fFIoSrJzathPhb3GGAGTgIYZz3fKi2LrBmbl7AYju6Zl0iTTxgj7ItbPVqZQ3mu5xKNFum6HeAYa2A-_kDim7VYmkTkj45nq0tvPtkNXQi2F0nrrWdtbn3KlXy8OD6GLVJFnl91xZ06jTheUeHIvc7_cfjASa1b0QXi8I58MJK16dXxMxDIzjOFOTtfOooQ6dnlM-URnTZgdOLKzXptcLDvfww3lrrbySDoDvo_Zg-UbG-b1FpeHdJW-m5404osp1UyezjZ7W0lwT4S6M9Z1UQM_IfRQpjVSdZtC2xGfDJr6YtAlw4uT5JGVWGUYN1vQu0u7yujRktFoVudS_Z6qtd9P1T_3Cf_jpUKuBU6Wo50ekinp61Mw_TZZrCyyWASYLlveICHm0BLl' \
      -H 'Cache-Control: no-cache' \
      -H 'Connection: keep-alive' \
      -H 'Content-Length: 1027' \
      -H 'Content-Type: application/json' \
      -H 'Host: wshycpl.puntaleonaonline.com' \
      -H 'Postman-Token: 4102dc2e-34ee-4890-8317-e4f754bb0203,79fc0f82-ac6c-4f28-9660-7a5cba1319d4' \
      -H 'User-Agent: PostmanRuntime/7.18.0' \
      -H 'cache-control: no-cache' \
      -d '{
      "numero": 1,
      "fecha": "2019-10-16T11:03:01.0819927-06:00",
      "nombre": "Carlos",
      "apellidos": "Loria",
      "email": "carlos@loria.com",
      "identificacion": "105610581",
      "codigoTarifa": "RACK",
      "descuento1": 0.0,
      "descuento2": 0.0,
      "fechaLlegada": "2019-12-22T00:00:00",
      "fechaSalida":  "2019-12-27T00:00:00",
      "telefono": "",
      "celular": "83811199",
      "codigoProcedencia": 188,
      "codigoAgencia": "DIRECTO",
      "emailUsuario": "soporte@aristoteles.info",
      "observaciones": "Favor buscar acceso silla de ruedas",
      "MontoTotal": 2077.87,
    
      "numeroAsignado": 0,
      "procesada": false,
      "anulada": false,
    
      "detalle": [
        {
          "numero": 1,
          "linea": 1,
          "codigoTipoHabitacion": 11,
          "cantidad": 1,
          "ocupacion": 2,
          "paxAdultos": 2,
          "paxNinos": 1
        },
        {
          "numero": 1,
          "linea": 2,
          "codigoTipoHabitacion": 12,
          "cantidad": 1,
          "ocupacion": 2,
          "paxAdultos": 2,
          "paxNinos": 0
        }
      ]
    }
    '


- **Respuesta esperada**


    {
        "numero": 1,
        "fecha": "2019-10-16T11:03:01.0819927-06:00",
        "nombre": "Carlos",
        "apellidos": "Loria",
        "email": "carlos@loria.com",
        "identificacion": "105610581",
        "codigoTarifa": "RACK",
        "descuento1": 0.0,
        "descuento2": 0.0,
        "fechaLlegada": "2019-12-22T00:00:00",
        "fechaSalida": "2019-12-27T00:00:00",
        "telefono": "",
        "celular": "83811199",
        "codigoProcedencia": 188,
        "codigoAgencia": "DIRECTO",
        "emailUsuario": "soporte@aristoteles.info",
        "observaciones": "Favor buscar acceso silla de ruedas",
        "MontoTotal": 2077.87,
        "numeroAsignado": 0,
        "procesada": false,
        "anulada": false,
        "detalle": [
            {
                "numero": 1,
                "linea": 1,
                "codigoTipoHabitacion": 11,
                "cantidad": 1,
                "ocupacion": 2,
                "paxAdultos": 2,
                "paxNinos": 1
            },
            {
                "numero": 1,
                "linea": 2,
                "codigoTipoHabitacion": 12,
                "cantidad": 1,
                "ocupacion": 2,
                "paxAdultos": 2,
                "paxNinos": 0
            }
        ]
    }



- ![Con este registro se agrega la reservación al sistema de reservaciones de Aristóteles.  ](D:\DocumentacionesWSHYCPL\ReservaPruebas.PNG)

  ```
  Así se mostrará en el sistema de reservaciones Aristóteles la reservacion agregada.
  ```

  

# Códigos de estado de respuesta HTTP

- Cualquier estado distinto al 200 debe ser considerado como un error en la solicitud.
