# SC-Frontend-Sprint01-Ejercicio01-ModeloBD
SC-Frontend-Sprint01-Ejercicio01-ModeloBD

----------------------------------------------

RELACION DE TABLAS
----------------------------------------------
Relación [Curso] - [Tema]:
Un curso puede tener varios temas
Un Tema en específico pertenece a un solo curso

Relación [Tema] - [Pregunta]
Un Tema en puede tener varias preguntas
Una Pregunta está asociada a un único tema

Relación [Pregunta] - [Respuesta]
Una Pregunta puede tener varias Respuestas
Una Respuesta está asociada a una única pregunta

Relación [Usuario] (Resgistro) y demás tablas
El usuario está asociado a todas las tablas antes mencionadas
Por ejemplo:
	Un curso debe haber sido registrado y/o modificado por un usuario (perfil: administrador)
	Un Tema de un curso debe haber sido registrado y/o modificado por un usuario (perfil: administrador)
	Así mismo las preguntas y respuestas han sido publicadas por un usuario. (perfil: alumno y administrador)
Nota:
	para el modelo de base de datos he obviado los enlaces de relación
	
Relación [Usuario] (likes y dislikes) - [Pregunta]
Un usuario puede dar like o dislike a varias preguntas
Así mismo una pregunta puede recibir varios likes o dislike de usuarios
Se resuelve:
Dado que hay una relación de muchos a muchos, se resuelve dicha relación con la tabla [Like_Usuario_Pregunta], donde se especifica el usuario, la pregunta y el estado de like y dislike del mismo

Relación [Usuario] (likes y dislikes) - [Respuesta]
Un usuario puede dar like o dislike a varias Respuestas
Así mismo una Respuesta puede recibir varios likes o dislike de usuarios
Se resuelve:
Dado que hay una relación de muchos a muchos, se resuelve dicha relación con la tabla [Like_Usuario_Respuesta], donde se especifica el usuario, la respuesta y el estado de like y dislike del mismo
