# Pago de cuota de Mantenimiento
Antes de registrar un pago de cuota de mantenimiento se debe realizar una consulta de las cuotas pendientes para un suscriptor. Resumimos en tres pasos:
  - Autorizacion
  - Consulta de cuotas pendientes del suscriptor
  - Enviar pago haciendo referencia al documento específico y al socio

# Consulta de cuotas pendientes
  - Permite obtener las cuotas pendientes de un suscriptor
    # endpoint
    http://wsHYCPL.puntaleonaonline.com/api/Cuotas/Pendientes

    # Ejemplo 
        curl -X POST\
        'http://wsHYCPL.puntaleonaonline.com/api/Cuotas/Pendientes?codigoAccion=239' \
        -H 'Accept: */*' \
        -H 'Accept-Encoding: gzip, deflate' \
        -H 'Authorization: Bearer c3SHZxyJDUp_ixYy6jdSXHnNfl-vG7A9bV-xmjT73LPUEayEKbmCGRHCCsaePK5w5q12lmXrewej7q5ZTkiGW2O_hsqGh476w6qCgKrcrv8WstaW6G8jUor2P7S3wo5tqs1CDMkzao5-Hn35QzTeIWFb06LMDwy1TxCokrM8DnU6DWHKN5qbYyBl6iJCuy9pKjTNRfKjzUhi8dL4Rz8L7LRnGuxG42VAmQ2UujFvd0-na7-Hrv5HMMPEu7rSGEGwpT39kJV8JHJQ1f1_L0eKvG95YWD-1rntHTz3Ot2cyIX2h7r-T8W8z8pIVOZvudKhAed9rAvVixgio-zfwQO2Q8t_85HOUn4me11Vbm2QH02fQtZei7Rtvwgp8B23fwsPqzZCDtJjfResXbp3oTa6u-Y6O_GegIylt-JNASprs0CtaQ1bDwH77wRJk2vcyTiy4qduILlt-H9XsI96aZSzTabfqPsYDnK8dnxYrYfT3-oX8btQX2GjJsGOjytEyXHy' \
        -H 'Cache-Control: no-cache' \
        -H 'Connection: keep-alive' \
        -H 'Content-Length: 22' \
        -H 'Content-Type: application/json' \
        -H 'Host: wshycpl.puntaleonaonline.com' \
        -H 'Postman-Token: fe93bbaa-af59-4377-9d6e-ba7e80d5cd4d,4e7273fd-1a48-44b1-a5d1-9722bb48979c' \
        -H 'User-Agent: PostmanRuntime/7.15.2' \
        -H 'cache-control: no-cache' \
        -d '{"codigoAccion":"230"}'
# Respuesta esperada 
-
        [{
    	"codigoAccion": 239,
    	"tipoDocumento": 1,
    	"numeroDocumento": "R630048   ",
    	"plazo": 30,
    	"esDolares": false,
    	"codigoEjecutivo": 1,
    	"fecha": "2019-06-01T00:00:00",
    	"monto": 73000.0000,
    	"saldo": 73000.0000,
    	"tipoCambio": 596.0000,
    	"porcentajeIVA": 0.0000,
    	"montoBruto": 73000.000000000000000,
    	"montoIVA": 0.000000000000000}, {
    	"codigoAccion": 239,
    	"tipoDocumento": 1,
    	"numeroDocumento": "R635771   ",
    	"plazo": 30,
    	"esDolares": false,
    	"codigoEjecutivo": 1,
    	"fecha": "2019-08-01T00:00:00",
    	"monto": 73000.0000,
    	"saldo": 73000.0000,
    	"tipoCambio": 576.0000,
    	"porcentajeIVA": 0.0000,
    	"montoBruto": 73000.000000000000000,
    	"montoIVA": 0.000000000000000}]

# Pagos de Mantenimiento: agregar un pago
    El registro del pago, debe hacer referencia a una cuota específica, es decir indicando el número de suscriptor (codigoAccion) y el número de documento de la cuota pendiente a cancelar.
# endpoint 
    http://wsHYCPL.puntaleonaonline.com/api/Cuotas/Pendientes

# Ejemplo 
    -curl -X POST\
    http://wsHYCPL.puntaleonaonline.com/api/PagosMantenimiento/AgregarPago/ \
    -H 'Accept: */*' \
    -H 'Accept-Encoding: gzip, deflate' \
    -H 'Authorization: Bearer c3SHZxyJDUp_ixYy6jdSXHnNfl-vG7A9bV-xmjT73LPUEayEKbmCGRHCCsaePK5w5q12lmXrewej7q5ZTkiGW2O_hsqGh476w6qCgKrcrv8WstaW6G8jUor2P7S3wo5tqs1CDMkzao5-Hn35QzTeIWFb06LMDwy1TxCokrM8DnU6DWHKN5qbYyBl6iJCuy9pKjTNRfKjzUhi8dL4Rz8L7LRnGuxG42VAmQ2UujFvd0-na7-Hrv5HMMPEu7rSGEGwpT39kJV8JHJQ1f1_L0eKvG95YWD-1rntHTz3Ot2cyIX2h7r-T8W8z8pIVOZvudKhAed9rAvVixgio-zfwQO2Q8t_85HOUn4me11Vbm2QH02fQtZei7Rtvwgp8B23fwsPqzZCDtJjfResXbp3oTa6u-Y6O_GegIylt-JNASprs0CtaQ1bDwH77wRJk2vcyTiy4qduILlt-H9XsI96aZSzTabfqPsYDnK8dnxYrYfT3-oX8btQX2GjJsGOjytEyXHy' \
    -H 'Cache-Control: no-cache' \
    -H 'Connection: keep-alive' \
    -H 'Content-Length: 230' \
    -H 'Content-Type: application/json' \
    -H 'Host: wshycpl.puntaleonaonline.com' \
    -H 'Postman-Token: 5286bf69-4674-4842-bf12-d1951b1e288b,5f96c0d3-b15f-4d45-b45d-fb38b2f21f37' \
    -H 'User-Agent: PostmanRuntime/7.15.2' \
    -H 'cache-control: no-cache' \
    -d '{
    "numeroDocumentoPago": "1234567890",
    "fechaPago": "2019-08-20T00:00:00",
    "montoRecibido": 73000.0000,
    	"codigoAccion": 239,
    "tipoDocumento": 1,
    "numeroDocumento": "R630048"}'

# Respuesta esperada : 
    Se retorna un status 200 (ok) con el registro del pago recibido cuando se agrega el mismo.
    {
    "numeroDocumentoPago": "1234567890",
    "fechaPago": "2019-08-20T00:00:00",
    "montoRecibido": 73000.0000,
    "codigoAccion": 239,
    "tipoDocumento": 1,
    "numeroDocumento": "R630048"}

# Error 409:
    status 409 Conflict
    Ocurre cuando se ha recibido un pago con el mismo numero de documento. Refleja que existe un conflicto por cuanto el registro ya existe.

# Error 404
    Statis 404 Not Found
    Ocurre cuando no se encuentra el suscriptor indicado o el número de documento indicado
