<h4>2.3.4 Empathy Mapping</h3>
<p><strong>Cliente</strong></p>
<img src="./imagenes/Empathy map cliente.png" width="500" height="500">
<p><strong>Vendedor</strong></p>
<img src="./imagenes/Empathy map vendedor.png" width="500" height="500">

<h4>2.3.5 As-Is Scenario Mapping</h3>
<p>Nicolas desea adquirir productos alimenticios para su consumo semanal.</p>
<img src="./imagenes/As-Is 1.jpg" width="500" height="500">
<p>Sofia desea vender sus productos cuya fecha de caducidad está por llegar.</p>
<img src="./imagenes/As-Is 2.jpg" width="500" height="500">

<h3>2.4 Ubiquitious language</h3>

<h2>Capitulo III: Requirements Specification</h2>
<h3>3.1 To-Be Scenario Mapping</h3>
<p>Nicolas desea adquirir productos alimenticios para su consumo semanal.</p>
<img src="./imagenes/To-Be 1.jpg" width="500" height="500">
<p>Sofia desea vender sus productos cuya fecha de caducidad está por llegar.</p>
<img src="./imagenes/To-Be 2.jpg" width="500" height="500">

<h3>3.2 User Stories</h3>
<table>
  <tr><th>Epic/User Story ID</th> <th>Titulo</th> <th>Descripcion</th></tr>
  <tr><th>EP001</th> <td>Mejora la experiencia del usuario</td> <td>Como usuario de EcoMarket quiero que la aplicación me ofrezca una experiencia intuitiva y agradable. Esto implica un sistema de perfiles funcionales, mejor autenticación, navegación de productos y tiendas sencillas y un sistema de notificaciones efectivas para mantenerme informado con todas las novedades de la plataforma.</td></tr>
  <tr><th>EP002</th> <td>Gestion de compras y productos</td> <td>Como usuario de EcoMarket, quiero administrar mis compras de forma eficiente: Agregar fácilmente productos al carrito, ver un resumen claro de mi compra y confirmar sin dificultad. Además, deseo revisar mi historial de compras para llevar un registro adecuado.</td></tr>
  <tr><th>EP003</th> <td>Gestion de metodos de pago</td> <td>Como usuario de EcoMarket, deseo gestionar los métodos de pago que utilice de forma segura, rápida y eficiente. Quiero agregar, modificar y eliminar métodos de pago para realizar transacciones de manera rápida.</td></tr>
  <tr><th>EP004</th> <td>Gestion de productos para vendedores</td> <td>Como vendedor de EcoMarket, deseo exhibir los productos que tenga para ofrecer en la aplicación. Deseo que la aplicación me facilite la exhibición de mis productos a través de imágenes y descripciones. A la vez, quiero poder gestionar los productos en exhibición que tenga.</td></tr>
  <tr><th>EP005</th> <td>Gestion de ventas de vendedor</td> <td>Como vendedor de EcoMarket, necesito que la aplicación me facilite la administración de mi cuenta. Quiero autenticarme de manera sencilla, modificar mi perfil, acceder a mi historial de ventas y gestionar métodos de pago específicos para vendedores de manera efectiva. </td></tr>
</table>

<table>
  <tr><th>User Story ID</th> <th>Titulo</th> <th>Descripcion</th> <th>Criterios de aceptacion</th> <th>Epic ID</th></tr>
  <tr><th colspan = "5">Segmento cliente</th></tr>
  <tr><th>US001</th> <td>Añadir un producto al carrito</td> <td>Como usuario, quiero poder agregar un producto a mi carrito de compras para luego revisar cual es el subtotal de los productos seleccionados.</td> 
<td><strong>Escenario 1:</strong> Selección y Agregado al Carrito  
  
  <strong>Given</strong> que el usuario está explorando la lista de productos disponibles,  
  <strong>When</strong> el usuario selecciona un producto de su agrado y lo agrega al carrito,  
  <strong>Then</strong> el producto se agrega exitosamente al carrito de compras.  
  
  <strong>Escenario 2</strong>: Producto no disponible  
  <strong>Given</strong> que el usuario está explorando la lista de productos disponibles,  
  <strong>And</strong> el producto seleccionado no está en stock o no está disponible,  
  <strong>When</strong> el usuario intenta agregar el producto al carrito,  
  <strong>Then</strong> se muestra un mensaje de error indicando que el producto no está disponible.  

  <Strong>Escenario 3</Strong>: Error al Agregar al Carrito  
  <strong>Given</strong> que el usuario está explorando la lista de productos disponibles,   
  <strong>When</strong> el usuario intenta agregar un producto al carrito y ocurre un error en el sistema,   
  <strong>Then</strong> se muestra un mensaje de error indicando que hubo un problema al agregar el producto al carrito.</td> <th>EP001</th></tr>

  <tr><th>US002</th> <td>Mostrar carrito de compras con resumen de orden y botón de pago</td> <td>Como usuario, deseo poder ver un resumen de mi compra en el carrito y tener un botón en el cual puedo seleccionar mis métodos de pago y realizarlo</td> 
    <td><strong>Escenario 1</strong>: Visualización del Carrito  
      
 <strong>Given</strong> que el usuario tiene productos en su carrito  
 <strong>When</strong> el usuario accede a la sección de carrito,  
 <strong>Then</strong> se muestra un resumen de los productos seleccionados y un botón de pago.  

<strong>Escenario 2</strong>: Realizar Pago  
<strong>Given</strong> que el usuario está revisando el resumen de la orden en el carrito  
<strong>When</strong> el usuario hace clic en el botón de pago,  
<strong>Then</strong> es redirigido a una pasarela de pago para completar la compra.  

<strong>Escenario 3</strong>: Carrito Vacío  
<strong>Given</strong> que el usuario no tiene productos en su carrito  
<strong>When</strong> el usuario accede a la sección de carrito,  
<strong>Then</strong> se muestra un mensaje indicando que el carrito está vacío.</td> <th>EP001</th></tr>
  
  <tr><th>US003</th> <td>Mostrar productos al realizar el inicio de sesión</td> <td>Como usuario, deseo que, al abrir la aplicación EcoMarket y realizar el inicio de mi sesion, se me muestre una selección de productos para explorar de manera rápida y conveniente</td> <td><strong>Escenario 1</strong>: Visualización de Productos al Iniciar Sesión  
    
<strong>Given</strong> que el usuario ha iniciado sesión en la aplicación EcoMarket, Cuando el usuario accede a la plataforma,  
<strong>Then</strong> se le muestra una selección de productos en la página principal para explorar y comprar de manera rápida y conveniente.  

<strong>Escenario 2:</strong> Exploración de Productos  
<strong>Given</strong> que el usuario ha iniciado sesión en la aplicación EcoMarket,  
<strong>When</strong> el usuario explora la selección de productos mostrados al iniciar sesión,  
<strong>Then</strong> puede ver imágenes, descripciones y precios de cada producto, facilitando la toma de decisiones de compra.  

<strong>Escenario 3:</strong> Adición de Producto al Carrito  
<strong>Given</strong> que el usuario ha iniciado sesión en la aplicación EcoMarket,  
<strong>When</strong> el usuario selecciona un producto y hace clic en "Agregar al carrito",  
<strong>Then</strong> el producto se agrega al carrito de compras, permitiendo al usuario revisar y completar fácilmente su compra en el futuro.  

<strong>Escenario 4:</strong> Acceso Rápido a Detalles del Producto  
<strong>Given</strong> que el usuario ha iniciado sesión en la aplicación EcoMarket,  
<strong>When</strong> el usuario hace clic en un producto para obtener más detalles,  
<strong>Then</strong> se muestra información detallada del producto, como características, opiniones de otros compradores y disponibilidad, ayudando al usuario a tomar una decisión informada de compra. </td> <th>EP001</th></tr>
  
  <tr><th>US004</th> <td>Mostrar una barra de navegación lateral con varias opciones</td> <td>Como usuario, quiero que la aplicación muestre una barra de navegación lateral en el lado izquierdo con diversas opciones fundamentales de la aplicación</td> <td><strong>Escenario 1:</strong> Visualización de la Barra de Navegación Lateral  
    
<strong>Given</strong>  que el usuario ha iniciado sesión en la aplicación EcoMarket,  
<strong>When</strong>  el usuario accede a la aplicación,  
<strong>Then</strong>  se le muestra una barra de navegación lateral en el lado izquierdo de la pantalla con opciones como página principal, bandeja de entrada, perfil, historial y cerrar sesión, para acceder rápidamente a estas secciones.</td> <th>EP001</th></tr>
  
  <tr><th>US005</th> <td>Ingreso en la aplicación EcoMarket</td> <td>Como usuario, quiero poder ingresar mi cuenta en la aplicación EcoMarket, utilizando mi correo electronico mi contraseña para acceder a todas las funcionalidades que la aplicación ofrece</td> <td><strong>Escenario 1:</strong>  Inicio de Sesión Exitoso 
  
<strong>Given</strong>  que el usuario está en la pantalla de inicio de sesión en EcoMarket,  
<strong>When</strong>  el usuario ingresa su correo electrónico y contraseña registrados de forma correcta,  
<strong>And</strong>  hace clic en el botón de inicio de sesión,  
<strong>Then</strong>  el sistema verifica las credenciales, autentica al usuario y le permite acceder a todas las funcionalidades y datos asociados con su cuenta.  

<strong>Escenario 2:</strong>  Credenciales Incorrectas  
<strong>Given</strong>  que el usuario está en la pantalla de inicio de sesión en EcoMarket,  
<strong>When</strong>  el usuario ingresa credenciales incorrectas, ya sea un correo electrónico no registrado o una contraseña incorrecta,  
<strong>Then</strong>  el sistema muestra un mensaje de error indicando que las credenciales son incorrectas  
<strong>And</strong>  solicita al usuario que las ingrese nuevamente.  

<strong>Escenario 3:</strong>  Correo Electrónico no Registrado  
<strong>Given</strong>  que el usuario está en la pantalla de inicio de sesión en EcoMarket,  
<strong>When</strong>  el usuario ingresa un correo electrónico que no está registrado en el sistema,  
<strong>Then</strong>  el sistema muestra un mensaje indicando que el correo electrónico no está asociado a ninguna cuenta  
<strong>And</strong>  sugiere crear una nueva cuenta.</td> <th>EP001</th></tr>
  
  <tr><th colspan = "5">Segmento vendedor</th></tr>
  <tr><th>US006</th> <td>Añadir un nuevo producto</td> <td>Como vendedor, deseo poder añadir un producto a la aplicación EcoMarket, para así poder exhibir los productos que tengo para ofrecer a los demás usuarios</td> <td><strong>Escenario 1</strong>: Acceso a la Función de Añadir Producto
    
<strong>Given</strong> que el vendedor está en la aplicación EcoMarket,  
<strong>When</strong> el vendedor navega a la sección de añadir un producto,  
<strong>Then</strong> la aplicación muestra la página para añadir un nuevo producto.  


<strong>Escenario 2:</strong>  Ingreso de Información del Producto  
<strong>Given</strong> que el vendedor está en la página para añadir un nuevo producto,  
<strong>When</strong> el vendedor ingresa la información esencial del producto, como nombre, descripción, precio, stock y fecha de caducidad,  
<strong>Then</strong> la aplicación permite al vendedor proporcionar los datos necesarios para agregar el producto al catálogo de venta.  

<strong>Escenario 3</strong> : Validación de la Información del Producto  
<strong>Given</strong> que el vendedor ha ingresado la información del producto,  
<strong>When</strong> el vendedor hace clic en "Guardar" para añadir el producto,  
<strong>Then</strong> la aplicación valida los datos ingresados para garantizar que sean correctos y completos.  

<strong>Escenario 4:</strong>  Guardar el Nuevo Producto  
<strong>Dado</strong> que la información del nuevo producto ha sido validada con éxito,  
<strong>Given</strong> el vendedor confirma y guarda la información del producto,  
<strong>Then</strong> la aplicación agrega el producto al catálogo de venta del vendedor  
<strong>And</strong> muestra un mensaje de confirmación.  

<strong>Escenario 5:</strong>  Cancelación de la Creación del Nuevo Producto  
<strong>Given</strong> que el vendedor está en la página para añadir un nuevo producto,  
<strong>When</strong> el vendedor decide cancelar la creación sin guardar los datos ingresados,  
<strong>Then</strong> la aplicación no agrega ningún producto  
<strong>And</strong> devuelve al vendedor a la lista de productos.</td> <th>EP004</th></tr>

  <tr><th>US007</th> <td>Mostrar mis productos al iniciar sesión</td> <td>Como vendedor, quiero que, al iniciar sesion en la aplicación EcoMarket, se me muestre la lista de los productos que tengo exhibidos en mi cuenta, para así poder gestionarlos de manera eficiente</td> <td><strong>Escenario 1:</strong> Acceso a la Lista de Productos
    
<strong>Given</strong> que el vendedor está en la aplicación EcoMarket,  
<strong>When</strong> el vendedor inicia sesión,  
<strong>Then</strong> la aplicación muestra la lista de productos que el vendedor tiene en venta.  

<strong>Escenario 2:</strong> Visualización de Detalles de los Productos  
<strong>Given</strong> que el vendedor está en la lista de sus productos,  
<strong>When</strong> el vendedor selecciona un producto específico,  
<strong>Then</strong> la aplicación muestra los detalles detallados de ese producto, como nombre, descripción, precio, stock y fecha de caducidad.  

<strong>Escenario 3:</strong> Edición de los Productos  
<strong>Given</strong> que el vendedor está en la lista de sus productos,  
<strong>When</strong> el vendedor elige editar un producto,  
<strong>Then</strong> la aplicación permite al vendedor editar la información y actualizar detalles como nombre, descripción, precio, stock y fecha de caducidad.  

<strong>Escenario 4:</strong> Eliminación de un Producto  
<strong>Given</strong> que el vendedor está en la lista de sus productos,  
<strong>When</strong> el vendedor decide eliminar un producto,  
<strong>Then</strong> la aplicación permite al vendedor eliminar el producto seleccionado de su lista de productos.</td> <th>EP004</th></tr>
  
  <tr><th>US008</th> <td>Ver perfil como vendedor</td> <td>Como vendedor, quiero tener acceso a mi perfil en mi cuenta en EcoMarket, para así poder editar mi perfil así como tener un reporte de todas las ventas que hice y poder gestionar todos los productos que tengo a la venta</td> <td><strong>Escenario 1:</strong>  Acceso al Perfil de Vendedor
    
<strong>Given</strong> que el vendedor está en la aplicación EcoMarket,  
<strong>When</strong> el vendedor navega a la sección de perfil,  
<strong>Then</strong> la aplicación muestra la página del perfil del vendedor.  

<strong>Escenario 2:</strong> Visualización de Información de la Cuenta de Vendedor  
<strong>Given</strong> que el vendedor está en la página de perfil de vendedor,  
<strong>When</strong> el vendedor accede a la sección de información de la cuenta,  
<strong>Then</strong> la aplicación muestra detalles relevantes sobre la cuenta del vendedor, como nombre, dirección, e información de contacto.  

<strong>Escenario 3:</strong> Visualización de Detalles de Contacto  
<strong>Given</strong> que el vendedor está en la página de perfil de vendedor,  
<strong>When</strong> el vendedor accede a la sección de detalles de contacto,  
<strong>Then</strong> la aplicación muestra la información de contacto del vendedor, como dirección de correo electrónico y número de teléfono.</td> <th>EP005</th></tr>
  
  <tr><th>US009</th> <td>Editar perfil como vendedor</td> <td>Como vendedor, necesito actualizar y mantener precisa mi información de perfil, incluyendo datos de contacto y descripción de la empresa, para asegurarme que los clientes siempre reciban información relevante y actualizada.</td> <td><strong>Escenario 1:</strong> Acceso a la Edición del Perfil
    
<strong>Given</strong> que el vendedor está en la aplicación EcoMarket,  
<strong>When</strong> el vendedor navega a la sección de edición de perfil,  
<strong>Then</strong> la aplicación muestra la página para editar el perfil del vendedor.  

<strong>Escenario 2:</strong> Edición de la Información del Perfil  
<strong>Given</strong> que el vendedor está en la página de edición del perfil,  
<strong>When</strong> el vendedor modifica la información existente en su perfil, como detalles de contacto y descripción de la empresa,  
<strong>Then</strong> la aplicación permite al vendedor realizar cambios en la información de su perfil.  

<strong>Escenario 3:</strong> Validación de la Información Editada del Perfil  
<strong>Given</strong> que el vendedor ha editado la información de su perfil,  
<strong>When</strong> el vendedor hace clic en "Guardar" para actualizar la información del perfil,  
<strong>Then</strong> la aplicación valida los datos editados para garantizar que sean correctos y completos.   

<strong>Escenario 4:</strong> Guardar Cambios en el Perfil   
<strong>Given</strong> que la información del perfil ha sido validada con éxito,  
<strong>When</strong> el vendedor confirma y guarda la información del perfil,  
<strong>Then</strong> la aplicación actualiza la información del perfil del vendedor   
<strong>And</strong>  muestra un mensaje de confirmación.  

<strong>Escenario 5:</strong> Confirmación de Cambios en el Perfil  
<strong>Given</strong> que el vendedor ha guardado los cambios en su perfil,  
<strong>When</strong> la aplicación ha actualizado la información con éxito,  
<strong>Then</strong> se muestra un mensaje de confirmación indicando que los cambios se han guardado y que el perfil está actualizado.</td> <th>EP005</th></tr>
  
  <tr><th>US010</th> <td>Registro de vendedor</td> <td>Como nuevo vendedor, deseo crear una cuenta en la aplicación EcoMarket proporcionando la información necesaria, incluyendo correo electrónico, nombre de empresa, RUC, dirección, teléfono y contraseña, para acceder a los servicios de la aplicación como vendedor.</td> <td><strong>Escenario 1:</strong> Acceso a la Página de Registro
    
<strong>Given</strong> que el nuevo vendedor está en la aplicación EcoMarket,  
<strong>When</strong> el vendedor navega a la página de registro,  
<strong>Then</strong> la aplicación muestra la página de registro para vendedores.  

<strong>Escenario 2</strong>: Ingreso de Información de Registro  
<strong>Given</strong> que el vendedor está en la página de registro,  
<strong>When</strong> el vendedor ingresa la información requerida, como correo, nombre de empresa, RUC, dirección, teléfono y contraseña,  
<strong>Then</strong> la aplicación permite al vendedor proporcionar la información necesaria para el registro.   

<strong>Escenario 3:</strong> Validación de la Información de Registro   
<strong>Given</strong> que el vendedor ha ingresado la información de registro,  
<strong>When</strong> el vendedor hace clic en "Registrarse",  
<strong>Then</strong> la aplicación valida los datos ingresados para garantizar que sean correctos y completos.   

<strong>Escenario 4:</strong> Creación de la Cuenta de Vendedor  
<strong>Given</strong> que la información de registro ha sido validada con éxito,  
<strong>When</strong> el vendedor confirma y crea la cuenta de vendedor,  
<strong>Then</strong> la aplicación registra al vendedor en la plataforma  
<strong>And</strong>  muestra un mensaje de confirmación.  

<strong>Escenario 5:</strong> Error en el Registro   
<strong>Given</strong> que la información de registro no es válida o está incompleta,  
<strong>When</strong> el vendedor intenta registrarse sin proporcionar datos válidos,  
<strong>Then</strong> la aplicación muestra un mensaje de error indicando que el registro ha fallado y qué campos deben corregirse.</td> <th>EP005</th></tr>
</table>

<h3>3.3 Impact Mapping</h3>
<p><strong>Cliente</strong></p>
<img src="./imagenes/Impact map 2.png" width="500" height="500">
<p><strong>Vendedor</strong></p>
<img src="./imagenes/Impact map 1.png" width="500" height="500">

<h3>3.4 Product Backlog</h3>
<table>
  <tr><th>User Story</th> <th>Titulo</th> <th>Descripcion</th> <th>Story Points</th></tr>
  <tr><th colspan = "5">Segemento Cliente</th></tr>
  <tr><th>US001</th> <td>Añadir un producto al carrito</td> <td>Como usuario, quiero poder agregar un producto a mi carrito de compras para luego revisar cual es el subtotal de los productos seleccionados.</td> <th>8</th></tr>
  <tr><th>US002</th> <td>Mostrar carrito de compras con resumen de orden y botón de pago</td> <td>Como usuario, deseo poder ver un resumen de mi compra en el carrito y tener un botón en el cual puedo seleccionar mis métodos de pago y realizarlo</td> <th>8</th></tr>
  <tr><th>US003</th> <td>Mostrar productos al realizar el inicio de sesión</td> <td>Como usuario, deseo que, al abrir la aplicación EcoMarket y realizar el inicio de mi sesion, se me muestre una selección de productos para explorar de manera rápida y conveniente</td> <th>5</th></tr>
  <tr><th>US004</th> <td>Mostrar una barra de navegación lateral con varias opciones</td> <td>Como usuario, quiero que la aplicación muestre una barra de navegación lateral en el lado izquierdo con diversas opciones fundamentales de la aplicación</td> <th>5</th></tr>
  <tr><th>US005</th> <td>Ingreso en la aplicación EcoMarket</td> <td>Como usuario, quiero poder ingresar mi cuenta en la aplicación EcoMarket, utilizando mi correo electronico mi contraseña para acceder a todas las funcionalidades que la aplicación ofrece</td> <th>5</th></tr>
  <tr><th colspan = "5">Segemento Vendedor</th></tr>
  <tr><th>US006</th> <td>Añadir un nuevo producto</td> <td>Como vendedor, deseo poder añadir un producto a la aplicación EcoMarket, para así poder exhibir los productos que tengo para ofrecer a los demás usuarios</td> <th>8</th></tr>
  <tr><th>US007</th> <td>Mostrar mis productos al iniciar sesión</td> <td>Como vendedor, quiero que, al iniciar sesion en la aplicación EcoMarket, se me muestre la lista de los productos que tengo exhibidos en mi cuenta, para así poder gestionarlos de manera eficiente</td> <th>5</th></tr>
  <tr><th>US008</th> <td>er perfil como vendedor</td> <td>Como vendedor, quiero tener acceso a mi perfil en mi cuenta en EcoMarket, para así poder editar mi perfil así como tener un reporte de todas las ventas que hice y poder gestionar todos los productos que tengo a la venta</td> <th>3</th></tr>
  <tr><th>US009</th> <td>Editar perfil como vendedor</td> <td>Como vendedor, necesito actualizar y mantener precisa mi información de perfil, incluyendo datos de contacto y descripción de la empresa, para asegurarme que los clientes siempre reciban información relevante y actualizada.</td> <th>3</th></tr>
  <tr><th>US010</th> <td>Registro de vendedor</td> <td>Como nuevo vendedor, deseo crear una cuenta en la aplicación EcoMarket proporcionando la información necesaria, incluyendo correo electrónico, nombre de empresa, RUC, dirección, teléfono y contraseña, para acceder a los servicios de la aplicación como vendedor.</td> <th>2</th></tr>
</table>
