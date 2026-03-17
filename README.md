# LorHels-Office





**🧑‍💻 1. Portal de Empleados (*Autoservicio*)**

Es la cara pública de la app, diseñada para que cualquier persona de la empresa pida lo que necesita sin complicarse la vida:



* **Catálogo Inteligente:** Los empleados ven el inventario disponible con tarjetas visuales. Tienen una **barra de búsqueda en tiempo real** y **filtros de categorías automáticos** que se crean solos según lo que haya en la base de datos.



* **Carrito de Solicitudes:** Pueden agregar insumos cuidando de no pasarse del stock real que hay en almacén.



* **Comprobantes Automáticos:** Al enviar la solicitud, la app les genera y descarga automáticamente un Recibo en PDF con diseño profesional, folio de transacción, fecha, departamento y los espacios para firmas físicas.





**🛡️ 2. Panel Maestro (*Administración*)**

Es el "cerebro" para la gente de almacén y contabilidad. Está **protegido con inicio de sesión real (*Correo y Contraseña*)** mediante Firebase Auth. Tiene tres módulos:



* **Gestión de Inventario:** El administrador puede crear, editar o eliminar insumos. La tabla avisa visualmente (con alertas en rojo) cuando un producto cae por debajo de su stock mínimo.



* **Cola de Despacho (*Tickets*):** Las solicitudes de los empleados caen aquí al instante. El admin puede marcar un ticket como "Entregado" para confirmar el despacho.



* **Devoluciones Parciales y Totales:** ¡La joya de la corona! Si un empleado devuelve material (como un proyector o cables que sobraron), el admin puede especificar exactamente la cantidad devuelta, y **la app suma ese stock de regreso a la base de datos** automáticamente, dejando constancia en el historial.



* **Dashboard Analítico:** Gráficas en tiempo real que muestran qué departamento consume más insumos y cómo está la salud del stock actual.





**📊 3. Integración con Excel (*La función "Enterprise"*)**

* **Importación Masiva:** En lugar de crear los productos uno por uno, el admin puede subir un archivo de Excel y la app crea o actualiza todo el inventario de golpe.



* **Exportación de Reportes:** Con un clic, se puede descargar el Inventario Actual o el Historial completo de Solicitudes (con detalles de quién pidió, qué día, y qué devolvió) en formato *.xlsx* para cruzar datos a fin de mes.





**⚙️ 4. Tecnología bajo el capó**

* **Base de datos en tiempo real:** Todo está conectado a **Firebase Firestore**. Si el admin actualiza el stock, al empleado se le refleja al instante sin tener que recargar la página.



* **Diseño Responsivo:** Creado con Tailwind CSS, lo que significa que la app se ve y funciona perfecto tanto en la computadora de la oficina como en una tablet o celular.

