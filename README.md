# consultas1_sql

# EJERCICIOS CONSULTAS SQL

#CONSULTAS SQL

![tabla usuario](img/tabla_usuario.png "Tabla usuario")

1. Para visualizar toda la información que contiene la tabla `usuario` se puede incluir con la instrucción SELECT el caracter '*' o cada uno de los campos de la tabla

`select * from usuario`

![Consulta 1](img/captura2.png "Consulta1")

2. Visualizar solamente la indentificación del usuario

`select identificacion from usuario`

![COnsulta 2](img/captura3.png "Consulta 2")

3. Si se desea obtener los registros cuya identificación sean mayores o iguales a 150; se debe utilizar la clausula WHERE que especifica las condiciones que deben los registros que se van a seleccionar.

`SELECT * FROM usuario WHERE identificacion>=`150`

![Consulta3](img/captura4.png "Consulta 3")