# consultas2_sql

1. Obtener la lista de los apellidos de todos los empleados.

`SELECT apellidos_empleados FROM Empleados´

![Consulta 1](imagen/Apellidos.png  "Consulta 1")

2. obtener los apellidos de todos los empleados sin repeticiones

SELECT DISTINCT apellidos_empleado FROM empleado;

![Consulta 2](imagen/apellidosdiferentes.png "Consulta 2")

3. Obtener todos los datos de los empleados que se apellidan 'Gomez'

SELECT DISTINCT apellidos_empleado FROM empleado WHERE apellidos_empleado

[Consulta 3](imagen/Apellidos_gomez.png  "Consulta 3")

4. Obtener todos los datos de los empleados que se apellidan "Diaz" y los que se apellidan "Rodriguez".  Usar OR o IN

 FROM Empleado WHERE apellidos_empleado = 'Diaz' OR apellidos_empleado = 'Rodriguez';

[Consulta 4](imagen/Apellidospng  "Consulta 4")

5. Obtener los nombres de los empleados que trabajan en el departamento 11

SELECT * FROM Empleado WHERE apellidos_empleado LIKE 'P%';

6. Obtener todos los datos de los empleados cuyo apellido empiece por 'P'

7. Obtener el presupuesto total de todos los departamentos.

8. Obtener el número de empleados de cada departamento.

9. Obtener un listado completo de empleados, incluyendo por cada empleado los datos del empleado y de su departamento.

SELECT empleado.*, departamento.* FROM empleado JOIN departamento ON empleado.id_departamento = departamento.id_departamento;

|[Consulta 9](imagen/9png  "Consulta 9")

10. Obtener un listado completo de empleados, incluyendo el nombre y apellidos del empleado junto al nombre y presupuesto de su departamento.

|[Consulta 10](imagen/10png  "Consulta 10")

 SELECT empleado.nombre_empleado, empleado.apellidos_empleado, departamento.nombre_departamento, Departamento.presupuesto_departamento FROM Empleado JOIN departamento ON empleado.id_departamento = departamento.id_departamento;

11. Obtener los nombres y apellidos de los empleados que trabajen en departamentos cuyo presupuesto sea mayor a 100000000

SELECT Empleado.nombre_empleado, Empleado.apellidos_empleado FROM Empleado JOIN Departamento ON Empleado.id_departamento = Departamento.id_departamento WHERE Departamento.presupuesto_departamento > 100000000;

|[Consulta 11](imagen/11png  "Consulta 11")


