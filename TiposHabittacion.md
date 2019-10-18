# API HYCPL - TiposHabitacion/Lista

### Introducción

El catálogo de tipos de habitación permite conocer los tipos de habitación.

Para obtener la lista general se facilita este end point.

### EndPoint Procedencias/Lista
```
http://wshycpl.puntaleonaonline.com/api/TiposHabitacion/Lista
```

**Ejemplo**

- cURL


    curl -X POST \
      http://wshycpl.puntaleonaonline.com/api/TiposHabitacion/Lista \
      -H 'Accept: */*' \
      -H 'Accept-Encoding: gzip, deflate' \
      -H 'Authorization: Bearer V7QkuF1pHLmIb7b46cMFlk0NpnKlYGgaEaMeVokkyzVcobtCChN18h8RvNkEm3XfSySl5pxMj1mx2zTV4o9P3M1rz4YoUGa0PnIN0iT4tIar4vAs0_56fFIoSrJzathPhb3GGAGTgIYZz3fKi2LrBmbl7AYju6Zl0iTTxgj7ItbPVqZQ3mu5xKNFum6HeAYa2A-_kDim7VYmkTkj45nq0tvPtkNXQi2F0nrrWdtbn3KlXy8OD6GLVJFnl91xZ06jTheUeHIvc7_cfjASa1b0QXi8I58MJK16dXxMxDIzjOFOTtfOooQ6dnlM-URnTZgdOLKzXptcLDvfww3lrrbySDoDvo_Zg-UbG-b1FpeHdJW-m5404osp1UyezjZ7W0lwT4S6M9Z1UQM_IfRQpjVSdZtC2xGfDJr6YtAlw4uT5JGVWGUYN1vQu0u7yujRktFoVudS_Z6qtd9P1T_3Cf_jpUKuBU6Wo50ekinp61Mw_TZZrCyyWASYLlveICHm0BLl' \
      -H 'Cache-Control: no-cache' \
      -H 'Connection: keep-alive' \
      -H 'Content-Length: 0' \
      -H 'Content-Type: application/json' \
      -H 'Host: wshycpl.puntaleonaonline.com' \
      -H 'Postman-Token: 36bb099d-1951-4ca4-b8d8-45dc63fc36f3,eef8b00b-0b85-4aac-b25a-16d72bdf8269' \
      -H 'User-Agent: PostmanRuntime/7.18.0' \
      -H 'cache-control: no-cache'


- **Respuesta esperada**


    [
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 11,
            "nombreTipoHabitacion": "SELVAMAR",
            "codigoCategoriaHabitacion": 1,
            "cantidadHabitaciones": 64,
            "capacidadPax": 3,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 2,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 10,
            "imagenId": 1,
            "codigoMensaje": 111
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 12,
            "nombreTipoHabitacion": "SELVAMAR SUPERIOR",
            "codigoCategoriaHabitacion": 1,
            "cantidadHabitaciones": 23,
            "capacidadPax": 3,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 0,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 10,
            "imagenId": 2,
            "codigoMensaje": 112
        },
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
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 14,
            "nombreTipoHabitacion": "SELVAMAR SUPERIOR BALCON",
            "codigoCategoriaHabitacion": 1,
            "cantidadHabitaciones": 15,
            "capacidadPax": 3,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 2,
            "cantidadCamasDobles": 0,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 10,
            "imagenId": 3,
            "codigoMensaje": 114
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 21,
            "nombreTipoHabitacion": "ARENAS",
            "codigoCategoriaHabitacion": 2,
            "cantidadHabitaciones": 6,
            "capacidadPax": 8,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 0,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 12,
            "imagenId": 6,
            "codigoMensaje": 121
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 22,
            "nombreTipoHabitacion": "CHALET DOS DORMITORIOS",
            "codigoCategoriaHabitacion": 2,
            "cantidadHabitaciones": 6,
            "capacidadPax": 8,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 4,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 12,
            "imagenId": 8,
            "codigoMensaje": 122
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 23,
            "nombreTipoHabitacion": "CHALET UN DORMITORIO",
            "codigoCategoriaHabitacion": 2,
            "cantidadHabitaciones": 6,
            "capacidadPax": 4,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 2,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 12,
            "imagenId": 7,
            "codigoMensaje": 123
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 25,
            "nombreTipoHabitacion": "TORREMAR",
            "codigoCategoriaHabitacion": 2,
            "cantidadHabitaciones": 6,
            "capacidadPax": 4,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 2,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 12,
            "imagenId": 9,
            "codigoMensaje": 125
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 31,
            "nombreTipoHabitacion": "CABANA UN DORMITORIO",
            "codigoCategoriaHabitacion": 3,
            "cantidadHabitaciones": 17,
            "capacidadPax": 4,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 2,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 13,
            "imagenId": -1,
            "codigoMensaje": 131
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 32,
            "nombreTipoHabitacion": "CABANA DOS DORMITORIOS",
            "codigoCategoriaHabitacion": 3,
            "cantidadHabitaciones": 3,
            "capacidadPax": 6,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 3,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 13,
            "imagenId": -1,
            "codigoMensaje": 132
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 33,
            "nombreTipoHabitacion": "CABANA REMODELADA UN DORMITORIO",
            "codigoCategoriaHabitacion": 3,
            "cantidadHabitaciones": 0,
            "capacidadPax": 4,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 2,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 13,
            "imagenId": -1,
            "codigoMensaje": 133
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 34,
            "nombreTipoHabitacion": "CABANA REMODELADA DOS DORMITORIOS",
            "codigoCategoriaHabitacion": 3,
            "cantidadHabitaciones": 0,
            "capacidadPax": 6,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 3,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 13,
            "imagenId": -1,
            "codigoMensaje": 134
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 41,
            "nombreTipoHabitacion": "DELUXE SUITE",
            "codigoCategoriaHabitacion": 4,
            "cantidadHabitaciones": 6,
            "capacidadPax": 4,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 0,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 14,
            "imagenId": -1,
            "codigoMensaje": 141
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 42,
            "nombreTipoHabitacion": "JUNIOR SUITE",
            "codigoCategoriaHabitacion": 4,
            "cantidadHabitaciones": 4,
            "capacidadPax": 4,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 0,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 14,
            "imagenId": -1,
            "codigoMensaje": 142
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 43,
            "nombreTipoHabitacion": "SENIOR SUITE",
            "codigoCategoriaHabitacion": 4,
            "cantidadHabitaciones": 2,
            "capacidadPax": 6,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 0,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 14,
            "imagenId": -1,
            "codigoMensaje": 143
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 44,
            "nombreTipoHabitacion": "DELUXE SUITE LQ",
            "codigoCategoriaHabitacion": 6,
            "cantidadHabitaciones": 0,
            "capacidadPax": 1,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 0,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 14,
            "imagenId": -1,
            "codigoMensaje": 144
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 51,
            "nombreTipoHabitacion": "BELLA LEONA",
            "codigoCategoriaHabitacion": 5,
            "cantidadHabitaciones": 2,
            "capacidadPax": 6,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 0,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 15,
            "imagenId": 5,
            "codigoMensaje": 151
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 61,
            "nombreTipoHabitacion": "CASA PGM",
            "codigoCategoriaHabitacion": 6,
            "cantidadHabitaciones": 1,
            "capacidadPax": 0,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 0,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 16,
            "imagenId": -1,
            "codigoMensaje": 161
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 62,
            "nombreTipoHabitacion": "SOTAVENTO-GC",
            "codigoCategoriaHabitacion": 6,
            "cantidadHabitaciones": 0,
            "capacidadPax": 0,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 0,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 16,
            "imagenId": -1,
            "codigoMensaje": 162
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 63,
            "nombreTipoHabitacion": "SOTAVENTO-GS",
            "codigoCategoriaHabitacion": 6,
            "cantidadHabitaciones": 1,
            "capacidadPax": 0,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 0,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 16,
            "imagenId": -1,
            "codigoMensaje": 163
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 64,
            "nombreTipoHabitacion": "SOTAVENTO-JA",
            "codigoCategoriaHabitacion": 6,
            "cantidadHabitaciones": 1,
            "capacidadPax": 0,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 0,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 16,
            "imagenId": -1,
            "codigoMensaje": 164
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 65,
            "nombreTipoHabitacion": "SOTAVENTO-LA",
            "codigoCategoriaHabitacion": 6,
            "cantidadHabitaciones": 0,
            "capacidadPax": 0,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 0,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 16,
            "imagenId": -1,
            "codigoMensaje": 165
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 66,
            "nombreTipoHabitacion": "SOTAVENTO-MS",
            "codigoCategoriaHabitacion": 6,
            "cantidadHabitaciones": 0,
            "capacidadPax": 0,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 0,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 16,
            "imagenId": -1,
            "codigoMensaje": 166
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 67,
            "nombreTipoHabitacion": "SOTAVENTO-IB             ",
            "codigoCategoriaHabitacion": 6,
            "cantidadHabitaciones": 1,
            "capacidadPax": 0,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 0,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 16,
            "imagenId": -1,
            "codigoMensaje": 167
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 68,
            "nombreTipoHabitacion": "GOLDEN REEF -SP",
            "codigoCategoriaHabitacion": 7,
            "cantidadHabitaciones": 1,
            "capacidadPax": 0,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 0,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 16,
            "imagenId": -1,
            "codigoMensaje": 168
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 69,
            "nombreTipoHabitacion": "CHALET DE MONTAÑA",
            "codigoCategoriaHabitacion": 6,
            "cantidadHabitaciones": 1,
            "capacidadPax": 0,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 0,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 16,
            "imagenId": -1,
            "codigoMensaje": 169
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 81,
            "nombreTipoHabitacion": "ARRECIFES MASTE6",
            "codigoCategoriaHabitacion": 8,
            "cantidadHabitaciones": 2,
            "capacidadPax": 6,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 0,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 18,
            "imagenId": -1,
            "codigoMensaje": 181
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 82,
            "nombreTipoHabitacion": "ARRECIFES ESTUDIO        ",
            "codigoCategoriaHabitacion": 8,
            "cantidadHabitaciones": 3,
            "capacidadPax": 4,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 0,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 18,
            "imagenId": -1,
            "codigoMensaje": 182
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 83,
            "nombreTipoHabitacion": "ARRECIFES APTO4          ",
            "codigoCategoriaHabitacion": 8,
            "cantidadHabitaciones": 13,
            "capacidadPax": 4,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 0,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 18,
            "imagenId": -1,
            "codigoMensaje": 183
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 84,
            "nombreTipoHabitacion": "ARRECIFES MASTE8",
            "codigoCategoriaHabitacion": 8,
            "cantidadHabitaciones": 2,
            "capacidadPax": 8,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 0,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 18,
            "imagenId": -1,
            "codigoMensaje": 184
        },
        {
            "hotel_id": 4,
            "codigoTipoHabitacion": 85,
            "nombreTipoHabitacion": "ARRECIFES APTO6          ",
            "codigoCategoriaHabitacion": 8,
            "cantidadHabitaciones": 12,
            "capacidadPax": 6,
            "cantidadCamasKing": 0,
            "cantidadCamasQueen": 0,
            "cantidadCamasDobles": 0,
            "cantidadCamasSecillas": 0,
            "enable": true,
            "codigoItemHospedaje": 18,
            "imagenId": -1,
            "codigoMensaje": 185
        }
    ]



# Códigos de estado de respuesta HTTP

Cualquier estado distinto al 200, debe considerarse como un error de la solicitud.

