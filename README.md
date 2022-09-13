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

4. Si se desea obtener los registros cuyosus apellidos sean Vanegas o Cetina, se debe utilizar el operador IN que especifica los registros que se quieren visualizar de una tabla.

`SELECT apellidos FROM usuario WHERE apellidos IN ('Vanegas','Cetina')`

![Consulta4](img/captura5.png "Consulta4")

`SELECT apellidos FROM usuario WHERE apellidos='Vanegas' OR apellidos='cetina'`

![Consulta4](img/captura6.png "Consulta4")

5. Si se desea obtener los registros cuya identificación sea menor de '110' y la ciudad sea 'Cali' se debe utilizar el operador AND.

`SELECT * FROM usuario WHERE identificacion<'110' AND ciudad_nac='Cali'`

![Consulta5](img/captura7.png "Consulta5")