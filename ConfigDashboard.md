# Añadir dashboard para gráfico de datos.

Los dashboards son bloques que consultan periódicamente la base de datos y grafican de forma elegante los datos, toda conguración se hace a través del aplicativo web.

- Acceder al dashboard
http://localhost:3000
*(user:pass in priv repo)*
- Una vez iniciada sesión como administrador, sigue:

## Añadir la base de datos

1. Panel lateral izquierdo > icono Configuration > Data Sources o http://localhost:3000/datasources
2. Hacer clic en el boton **[Add data source]**
3. Buscar y seleccionar el tipo de base de datos, *(MySQL funciona igual para MariaDB)*.
4. Aparecerá un formulario con campos por rellenar, diligenciar segun la base de datos.
5. Hacer clic en **[Save & test]**, debe salir un mensaje: *Database Connection OK*

![add database mysql](/imgs/addDB.gif)

## Crear un dashboard

1. Panel lateral izquierdo > icono Create > Dashboard o http://localhost:3000/dashboard/new
2. Se desplegará una interfaz interactiva que lleva por título New dashboard; en la parte superior derecha aparecen unos íconos, el primero [Add panel] añade los gráficos y el siguiente [Save dashboard] es importante ya que si no se presiona no se guardan los cambios.
3. Presionar *Add panel* y luego en el recuadro grande *Add an empty panel*
4. En la parte inferior izquierda apareceran las bases de datos disponibles, seleccionar la adecuada.
5. Configurar el query, se selecciona una tabla, importante, seleccionar una comlumna de tiempo y la columna de datos requerida.
6. Una vez realizada correctamente la consulta a la base de datos la gráfica se genera.
7. Los datos se pueden ajustar dentro del mismo query o mediante una expresión matemática.
8. Finalmente en la parte superior derecha presionar en **[Apply]** y en el dashboard **[Save dashboard]**.

![panels dashboard1](/imgs/dash1.gif)
![panels dashboard2](/imgs/dash2.gif)
![panels dashboard3](/imgs/dash3.gif)

## Crear un usuario cliente

1. Panel lateral izquierdo > icono Server Admin > Users o http://localhost:3000/admin/users
2. Presionar en **[New user]** y diligenciar los datos del formulario, *(El correo que se pide no tiene porqué ser real)*.
3. Al dar **[Create user]** se creará un usuario que por defecto es cliente.

![add user](/imgs/user.gif)

## Crear un Team
El team tiene la finalidad de compatir los dashboards creados con los usuarios cliente.

1. Panel lateral izquierdo > icono Configuration > Teams o http://localhost:3000/org/teams
2. Diligenciar los datos y crear.
3. Nuevamente al ingresar a Teams aparecerá el Team creado, dar clic y añadir a los clientes.
4. En la pestaña **Settings**, *debajo del nombre del Team* se puede cambiar el dashboard que carga una vez se inicia sesión por parte de un cliente.
5. Por tanto si se desea mostar una estación en específico, hacer clic en Settings, bajar y buscar **Preferences** y en Home Dashboard, elegir el deseado.
6. Finalmente guardar.

![add team](/imgs/team.gif)
