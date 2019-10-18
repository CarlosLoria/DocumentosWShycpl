# API HYCPL - TiposHabitacion/Leer

### Introducción

El catálogo de tipos de habitación permite conocer los tipos de habitación.

Para leer un tipo de habitación en particular, debe indicarse el código del tipo de habitación.

### EndPoint Procedencias/Leer
```
http://wshycpl.puntaleonaonline.com/api/TiposHabitacion/Leer?codigoTipoHabitacion={id}
```

**Ejemplo**

- cURL


    curl -X POST \
      'http://wshycpl.puntaleonaonline.com/api/TiposHabitacion/Leer?codigoTipoHabitacion=13' \
      -H 'Accept: */*' \
      -H 'Accept-Encoding: gzip, deflate' \
      -H 'Authorization: Bearer V7QkuF1pHLmIb7b46cMFlk0NpnKlYGgaEaMeVokkyzVcobtCChN18h8RvNkEm3XfSySl5pxMj1mx2zTV4o9P3M1rz4YoUGa0PnIN0iT4tIar4vAs0_56fFIoSrJzathPhb3GGAGTgIYZz3fKi2LrBmbl7AYju6Zl0iTTxgj7ItbPVqZQ3mu5xKNFum6HeAYa2A-_kDim7VYmkTkj45nq0tvPtkNXQi2F0nrrWdtbn3KlXy8OD6GLVJFnl91xZ06jTheUeHIvc7_cfjASa1b0QXi8I58MJK16dXxMxDIzjOFOTtfOooQ6dnlM-URnTZgdOLKzXptcLDvfww3lrrbySDoDvo_Zg-UbG-b1FpeHdJW-m5404osp1UyezjZ7W0lwT4S6M9Z1UQM_IfRQpjVSdZtC2xGfDJr6YtAlw4uT5JGVWGUYN1vQu0u7yujRktFoVudS_Z6qtd9P1T_3Cf_jpUKuBU6Wo50ekinp61Mw_TZZrCyyWASYLlveICHm0BLl' \
      -H 'Cache-Control: no-cache' \
      -H 'Connection: keep-alive' \
      -H 'Content-Length: 0' \
      -H 'Content-Type: application/json' \
      -H 'Host: wshycpl.puntaleonaonline.com' \
      -H 'Postman-Token: 21617bec-39c9-4e44-90c7-7f6600c318f0,d8a03250-3c1c-4d54-ba3c-dbbe8c319c29' \
      -H 'User-Agent: PostmanRuntime/7.18.0' \
      -H 'cache-control: no-cache'


- **Respuesta esperada**


    {
        "hotel_id": 4,
        "codigoTipoHabitacion": 13,
        "nombreTipoHabitacion": "SELVAMAR SUPERIOR KING BALCON",
        "codigoCategoriaHabitacion": 1,
        "cantidadHabitaciones": 5,
        "capacidadPax": 2,
        "cantidadCamasKing": 0,
        "cantidadCamasQueen": 0,
        "cantidadCamasDobles": 0,
        "cantidadCamasSecillas": 0,
        "enable": true,
        "codigoItemHospedaje": 10,
        "imagenId": 4,
        "codigoMensaje": 113
    }



# Códigos de estado de respuesta HTTP

Cualquier estado distinto al 200, debe considerarse como un error de la solicitud.

​	404 Not Found se envía cuando no existe el código indicado.

