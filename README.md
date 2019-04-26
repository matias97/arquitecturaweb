# arquitecturaweb

Trabajo Practico arquitectura web

Integrantes del grupo: Matias de la Serna - Ignacio Gonzalez

Negocio: Reservas de canchas de futbol.



Endpoints:

Grupos: 

Lugares: Create, Read, Update, Delete, List, Image. Estos son los diferentes establecimientos que ofrecen sus canchas para reservar. Se pueden filtrar por tamaño, disponibilidad y zona.

Zonas: Create, Read, Update, Delete, List. Estas son las zonas en las que existen canchas para reservar.

Users: Create, Read, Update, Delete, List, Image.

Reservas: Create, Read, Update, Delete, List.


GET's:

Zonas:

GET /zonas - Lista todas las zonas disponibles.

GET /zonas/x/lugares/y,z - Busca establecimientos en una zona específica, pudiendo filtrar por tamaño y/o disponibilidad.

Lugares:

GET /lugares - Lista todos los establecimientos.

GET /lugares/x,y - Busca un establecimiento específico (en todas las zonas), pudiendo filtrar ya sea por tamaño de la cancha y/o disponibilidad.

GET /lugares/x/reservas - Devuelve las reservas que existen en el establecimiento específico.

Users:

GET /users - Devuelve todos los usuarios.

GET /users/x - Devuelve el usuario específico.

GET /users/x/reservas - Devuelve las reservas del usuario específico.

Reservas:

GET /reservas - Devuelve todas las reservas.

GET /reservas/x - Devuelve la reserva específica.

GET /reservas/zonas/x - Devuelve las reservas de la zona específica.


POST's:

POST /zonas - Crea una nueva zona.

POST /lugares - Crea un nuevo lugar.

POST /users - Crea un nuevo usuario.

POST /users/x/reservas - Crea una nueva reserva para un usuario.


DELETE's:

DELETE /zonas/x - Elimina una zona especifica.

DELETE /zonas/x,y,z - Elimina las zonas especificadas.

DELETE /lugares/x - Elimina el establecimiento especifico.

DELETE /lugares/x,y,z - Elimina los lugares especificados.

DELETE /users/x - Elimina el usuario especifico.

DELETE /users/x,y,z - Elimina los usuarios especificados.

DELETE /reservas/x - Elimina la reserva especifica.

DELETE /reservas/x,y,z - Elimina las reservas especificadas.


PUT's:

PUT /lugares/x/imagen - Modifica la imagen del establecimiento.


PUT /users/x/imagen - Modifica la imagen del usuario.




