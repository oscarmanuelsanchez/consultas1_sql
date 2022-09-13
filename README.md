# consultas1_sql

# EJERCICIOS CONSULTAS SQL

#CONSULTAS SQL


![tabla usuario](img/tabla_usuario.png "Tabla usuario")
## COMANDO SELECT

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
6. Si se desea obtener los registros cuyos nombres empiecen por la letra 'A', se debe utilizar el operador LIKE que utiliza los patrones '%' (todos) y '_' (caracter).

`SELECT * FROM usuario WHERE nombre LIKE 'A%'`

![Consulta6](img/captura8.png "Consulta6")

7. Si se desea obtener los registros cuos nombres contengan la letra 'a'.
`SELECT * FROM usuario WHERE nombre LIKE '%a%'`

![Consulta7](img/captura9.png "Consulta7")

8. Si se desea obtener los registros donde la cuarta letra del nombre sea una 'a'.

`SELECT * FROM usuario WHERE nombre LIKE '___a%'`

![Consulta8](img/captura10.png "Consulta8")

9. Si se desea obtener los registros cuya identificacion este en el inventario 110 y 150, se debee utilizar la cláusula BETWEEN, que sirve para especificar un intervalo de valores.

`SELECT * FROM usuario WHERE Identificación BETWEEN '110' and '150'`

![Consulta9](img/captura11.png "Consulta9")