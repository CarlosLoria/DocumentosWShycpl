# API HYCPL - Tarifas/Lista

### Introducción

El catálogo de tarifas permite indicar las tarifas activas para el portal.

Para obtener una lista general utilice este endpoint.

### EndPoint Tarifas/Lista
```
http://wshycpl.puntaleonaonline.com/api/Tarifas/Lista
```

**Ejemplo**

- cURL


    curl -X POST \
      http://wshycpl.puntaleonaonline.com/api/Tarifas/Lista \
      -H 'Accept: */*' \
      -H 'Accept-Encoding: gzip, deflate' \
      -H 'Authorization: Bearer V7QkuF1pHLmIb7b46cMFlk0NpnKlYGgaEaMeVokkyzVcobtCChN18h8RvNkEm3XfSySl5pxMj1mx2zTV4o9P3M1rz4YoUGa0PnIN0iT4tIar4vAs0_56fFIoSrJzathPhb3GGAGTgIYZz3fKi2LrBmbl7AYju6Zl0iTTxgj7ItbPVqZQ3mu5xKNFum6HeAYa2A-_kDim7VYmkTkj45nq0tvPtkNXQi2F0nrrWdtbn3KlXy8OD6GLVJFnl91xZ06jTheUeHIvc7_cfjASa1b0QXi8I58MJK16dXxMxDIzjOFOTtfOooQ6dnlM-URnTZgdOLKzXptcLDvfww3lrrbySDoDvo_Zg-UbG-b1FpeHdJW-m5404osp1UyezjZ7W0lwT4S6M9Z1UQM_IfRQpjVSdZtC2xGfDJr6YtAlw4uT5JGVWGUYN1vQu0u7yujRktFoVudS_Z6qtd9P1T_3Cf_jpUKuBU6Wo50ekinp61Mw_TZZrCyyWASYLlveICHm0BLl' \
      -H 'Cache-Control: no-cache' \
      -H 'Connection: keep-alive' \
      -H 'Content-Length: 0' \
      -H 'Content-Type: application/json' \
      -H 'Host: wshycpl.puntaleonaonline.com' \
      -H 'Postman-Token: 826884c8-bd98-4660-8dd2-276601acb048,f3998276-ed9e-4597-8546-9afd1a31bc7e' \
      -H 'User-Agent: PostmanRuntime/7.18.0' \
      -H 'cache-control: no-cache'


- **Respuesta esperada**


    [
        {
            "codigoTarifa": "A-20%  ",
            "nombreTarifa": "AGENCIA 20%COMISION ",
            "enable": true
        },
        {
            "codigoTarifa": "A-25%  ",
            "nombreTarifa": "AGENCIAS 25% COMISION ",
            "enable": true
        },
        {
            "codigoTarifa": "A-30%  ",
            "nombreTarifa": "AGENCIA 30% COMISION ",
            "enable": true
        },
        {
            "codigoTarifa": "CPL-CLU",
            "nombreTarifa": "CPL CLUB INCENTIVO MIEMBRO",
            "enable": true
        },
        {
            "codigoTarifa": "RACK   ",
            "nombreTarifa": "Tarifa Rack",
            "enable": true
        },
        {
            "codigoTarifa": "SOCIOS ",
            "nombreTarifa": "Tarifa especial para socios",
            "enable": true
        }
    ]



# Códigos de estado de respuesta HTTP

Cualquier estado distinto al 200, debe considerarse como un error de la solicitud.

