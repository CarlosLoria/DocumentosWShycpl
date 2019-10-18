# API HYCPL - Tarifas/TarifaDiaria

### Introducción

El catálogo de tarifas permite indicar las tarifas activas para el portal. La consulta de tarifa diaria permite obtener los importes que de cobran por fecha en la tarifa indicada.

### EndPoint Tarifas/TarifaDiaria
```
http://wshycpl.puntaleonaonline.com/api/Tarifas/TarifaDiaria
```

**Ejemplo**

- cURL


    curl -X POST \
      http://wshycpl.puntaleonaonline.com/api/Tarifas/TarifaDiaria \
      -H 'Accept: */*' \
      -H 'Accept-Encoding: gzip, deflate' \
      -H 'Authorization: Bearer V7QkuF1pHLmIb7b46cMFlk0NpnKlYGgaEaMeVokkyzVcobtCChN18h8RvNkEm3XfSySl5pxMj1mx2zTV4o9P3M1rz4YoUGa0PnIN0iT4tIar4vAs0_56fFIoSrJzathPhb3GGAGTgIYZz3fKi2LrBmbl7AYju6Zl0iTTxgj7ItbPVqZQ3mu5xKNFum6HeAYa2A-_kDim7VYmkTkj45nq0tvPtkNXQi2F0nrrWdtbn3KlXy8OD6GLVJFnl91xZ06jTheUeHIvc7_cfjASa1b0QXi8I58MJK16dXxMxDIzjOFOTtfOooQ6dnlM-URnTZgdOLKzXptcLDvfww3lrrbySDoDvo_Zg-UbG-b1FpeHdJW-m5404osp1UyezjZ7W0lwT4S6M9Z1UQM_IfRQpjVSdZtC2xGfDJr6YtAlw4uT5JGVWGUYN1vQu0u7yujRktFoVudS_Z6qtd9P1T_3Cf_jpUKuBU6Wo50ekinp61Mw_TZZrCyyWASYLlveICHm0BLl' \
      -H 'Cache-Control: no-cache' \
      -H 'Connection: keep-alive' \
      -H 'Content-Length: 132' \
      -H 'Content-Type: application/json' \
      -H 'Host: wshycpl.puntaleonaonline.com' \
      -H 'Postman-Token: b8c4afd8-6916-4da5-93f6-7dc9350fc825,53b9e81e-c5da-4586-807c-d5cb398caec9' \
      -H 'User-Agent: PostmanRuntime/7.18.0' \
      -H 'cache-control: no-cache' \
      -d '{
     "codigoTarifa":"RACK",
     "codigoTipoHabitacion":13,
     "fechaDesde": "2019-12-22T00:00:00",
     "fechaHasta": "2019-12-27T00:00:00",
    }
    '


- **Respuesta esperada**


    [
        {
            "codigoTarifa": "Rack   ",
            "codigoTipoHabitacion": 13,
            "fecha": "2019-12-22T00:00:00",
            "ADIadulto": 0.0000,
            "ADInino": 9.0000,
            "sencilla": 164.9800,
            "doble": 193.2300,
            "triple": 0.0000,
            "completa": 0.0000,
            "aplicaMealPlan": true,
            "descuentoES": 0.0000000
        },
        {
            "codigoTarifa": "Rack   ",
            "codigoTipoHabitacion": 13,
            "fecha": "2019-12-23T00:00:00",
            "ADIadulto": 0.0000,
            "ADInino": 9.0000,
            "sencilla": 164.9800,
            "doble": 193.2300,
            "triple": 0.0000,
            "completa": 0.0000,
            "aplicaMealPlan": true,
            "descuentoES": 0.0000000
        },
        {
            "codigoTarifa": "Rack   ",
            "codigoTipoHabitacion": 13,
            "fecha": "2019-12-24T00:00:00",
            "ADIadulto": 0.0000,
            "ADInino": 9.0000,
            "sencilla": 164.9800,
            "doble": 193.2300,
            "triple": 0.0000,
            "completa": 0.0000,
            "aplicaMealPlan": true,
            "descuentoES": 0.0000000
        },
        {
            "codigoTarifa": "Rack   ",
            "codigoTipoHabitacion": 13,
            "fecha": "2019-12-25T00:00:00",
            "ADIadulto": 0.0000,
            "ADInino": 9.0000,
            "sencilla": 206.7900,
            "doble": 241.8200,
            "triple": 0.0000,
            "completa": 0.0000,
            "aplicaMealPlan": true,
            "descuentoES": 0.0000000
        },
        {
            "codigoTarifa": "Rack   ",
            "codigoTipoHabitacion": 13,
            "fecha": "2019-12-26T00:00:00",
            "ADIadulto": 0.0000,
            "ADInino": 9.0000,
            "sencilla": 206.7900,
            "doble": 241.8200,
            "triple": 0.0000,
            "completa": 0.0000,
            "aplicaMealPlan": true,
            "descuentoES": 0.0000000
        }
    ]



# Códigos de estado de respuesta HTTP

Cualquier estado distinto al 200, debe considerarse como un error de la solicitud.

