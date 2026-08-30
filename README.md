My ToDo List App (MIT App Inventor)

Aplicación móvil interactiva de lista de tareas (To-Do List) desarrollada en MIT App Inventor. Permite la gestión completa de tareas cotidianas mediante la creación, lectura, actualización y eliminación de elementos (operaciones CRUD), garantizando la persistencia de datos local en el dispositivo.

Autora: Brenda Arana Gutiérrez

Descripción del Proyecto
La aplicación está diseñada para ayudar a los usuarios a administrar sus actividades diarias de manera intuitiva. Utiliza componentes de interfaz modular y la base de datos local TinyDB para almacenar y recuperar la lista de tareas incluso cuando la aplicación se cierra o se reinicia el dispositivo.


Características Principales

Agregar Tareas (Create): Permite ingresar un nuevo elemento desde un campo de texto y añadirlo dinámicamente a la lista global.
Visualización (Read): Muestra los elementos almacenados de forma ordenada utilizando el componente ListView.
Edición y Actualización (Update): Permite seleccionar un elemento existente de la lista, transferirlo a la vista de edición y guardar los cambios realizados.
Eliminación de Tareas (Delete): Facilita la remoción de tareas completadas o descartadas de la lista global y de la base de datos.
Persistencia de Datos: Integración con TinyDB utilizando la clave/etiqueta "Tasks" para sincronizar los cambios de forma permanente en el almacenamiento local.

Lógica de Programación y Bloques Implementados

La arquitectura de bloques de la aplicación abarca los siguientes eventos principales:

Screen1.Initialize: Al iniciar la aplicación, recupera la lista de tareas guardada en TinyDB bajo la etiqueta "Tasks" (si no existe, crea una lista vacía) y actualiza los elementos del ListView.
btnAddBtn.Click: Toma el texto del TextBox, lo añade a la lista global taskList, limpia el campo de texto y guarda el estado actualizado en TinyDB.
btnDelete.Click: Identifica el índice del elemento seleccionado en el ListView, lo remueve de taskList y actualiza TinyDB.
btnEdit.Click / btnSubmit.Click: Transiciona entre pantallas o contenedores de interfaz (MainScreen y EditScreen) para modificar una tarea seleccionada y sobrescribir el registro correspondiente.
