# Especificaciones API

A continuación se detallan los siguientes mensajes que tiene el API Stockist Phoenix.

Consta de los siguientes mensajes: 
- PhoenixHotelConfigurationRequest / PhoenixHotelConfigurationRequest 
	Mensaje dedicado a recuperar las habitaciones y tarifas de un hotel del cliente.
- PhoenixRoomRateUpdateRequest / PhoenixRoomRateUpdateResponse
	Mensaje dedicado a la publicación de precio, inventario, restricciones,... 
- PhoenixBookingNotificationRequest / PhoenixBookingNotificationResponse
	Mensaje dedicado a la notificación de reservas. El cliente envía el mensaje PhoenixBookingNotificationRequest con la reserva y espera la respuesta PhoenixBookingNotificationResponse
	
Es importante indicar que en cualquiera de las respuestas (Response) de estos mensajes podría indicarse que se ha producido un error al tratar la petición (Request). 
Los errores siempre se informarán siguiendo el elemento Error de la API. 
En el anexo final podrá observar algunos ejemplos. 