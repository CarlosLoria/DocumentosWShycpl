# API HYCPL - NochesLibres/Rango

### Introducción

La consulta de disponibilidad se realiza indicando un rango de fechas para un tipo de habitación.

### EndPoint NochesLibres/Rango
```
http://wshycpl.puntaleonaonline.com/api/NochesLibres/Rango
```

**Ejemplo**

- cURL


    curl -X POST \
      http://wshycpl.puntaleonaonline.com/api/NochesLibres/Rango \
      -H 'Accept: */*' \
      -H 'Accept-Encoding: gzip, deflate' \
      -H 'Authorization: Bearer V7QkuF1pHLmIb7b46cMFlk0NpnKlYGgaEaMeVokkyzVcobtCChN18h8RvNkEm3XfSySl5pxMj1mx2zTV4o9P3M1rz4YoUGa0PnIN0iT4tIar4vAs0_56fFIoSrJzathPhb3GGAGTgIYZz3fKi2LrBmbl7AYju6Zl0iTTxgj7ItbPVqZQ3mu5xKNFum6HeAYa2A-_kDim7VYmkTkj45nq0tvPtkNXQi2F0nrrWdtbn3KlXy8OD6GLVJFnl91xZ06jTheUeHIvc7_cfjASa1b0QXi8I58MJK16dXxMxDIzjOFOTtfOooQ6dnlM-URnTZgdOLKzXptcLDvfww3lrrbySDoDvo_Zg-UbG-b1FpeHdJW-m5404osp1UyezjZ7W0lwT4S6M9Z1UQM_IfRQpjVSdZtC2xGfDJr6YtAlw4uT5JGVWGUYN1vQu0u7yujRktFoVudS_Z6qtd9P1T_3Cf_jpUKuBU6Wo50ekinp61Mw_TZZrCyyWASYLlveICHm0BLl' \
      -H 'Cache-Control: no-cache' \
      -H 'Connection: keep-alive' \
      -H 'Content-Length: 109' \
      -H 'Content-Type: application/json' \
      -H 'Host: wshycpl.puntaleonaonline.com' \
      -H 'Postman-Token: 9eb23d9d-e159-4b6c-9a64-e5aa04e529f8,69230a44-1848-40c8-95bc-e2a4ad292263' \
      -H 'User-Agent: PostmanRuntime/7.18.0' \
      -H 'cache-control: no-cache' \
      -d '{
      "codigoTipoHabitacion":13,
     "fechaDesde": "2019-12-22T00:00:00",
     "fechaHasta": "2019-12-27T00:00:00",
    }
    '


- **Respuesta esperada**


    [
        {
            "hotel_id": 4,
            "Fecha": "2019-12-22T00:00:00",
            "codigoTipoHabitacion": 13,
            "Libres": 3
        },
        {
            "hotel_id": 4,
            "Fecha": "2019-12-23T00:00:00",
            "codigoTipoHabitacion": 13,
            "Libres": 4
        },
        {
            "hotel_id": 4,
            "Fecha": "2019-12-24T00:00:00",
            "codigoTipoHabitacion": 13,
            "Libres": 4
        },
        {
            "hotel_id": 4,
            "Fecha": "2019-12-25T00:00:00",
            "codigoTipoHabitacion": 13,
            "Libres": 4
        },
        {
            "hotel_id": 4,
            "Fecha": "2019-12-26T00:00:00",
            "codigoTipoHabitacion": 13,
            "Libres": 4
        }
    ]



# Códigos de estado de respuesta HTTP

Cualquier estado distinto al 200, debe considerarse como un error de la solicitud.

