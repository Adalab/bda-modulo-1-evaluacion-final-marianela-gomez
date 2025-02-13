# Table of contents

- [Spanish version](#ejercicio-evaluación-módulo-1-bootcamp-data-analytics-adalab)

- [English version](#final-exercise-module-1-adalab-data-analytics-bootcamp)

## Ejercicio evaluación Módulo 1 Bootcamp Data Analytics Adalab

Este repositorio contiene el ejercicio de evaluación del Módulo 1 (Python Básico) del Bootcamp de Data Analytics de Adalab. También incluye un archivo borrador (draft), dónde se recogen algunas pruebas hechas durante el desarrollo del código. 

El ejercicio consiste en crear la clase TiendaOnline y tiene la siguiente estructura: 

**Clase**: TiendaOnline

**Atributos**:
- inventario: Lista de diccionarios con productos (nombre, precio, cantidad).
- ventas_totales: float, inicializado en 0.

**Métodos**:

- `agregar_producto(nombre, precio, cantidad)`

    Si el producto ya existe, actualiza la cantidad.
    Si no, agrega un nuevo producto.
    
- `ver_inventario()`

    Muestra todos los productos del inventario.

- `buscar_producto(nombre)`

    Busca el producto por su nombre y muestra detalles si se encuentra.

- `actualizar_stock(nombre, cantidad)`

    Actualiza la cantidad de un producto existente.
    Si no está en el inventario, muestra un mensaje.

- `eliminar_producto(nombre)`

    Elimina un producto por nombre si existe.
    Muestra un mensaje si no se encuentra.

- `calcular_valor_inventario()`

    Calcula el valor total del inventario como:

    $$
    \sum Valor_{total} = precio*cantidad 
    $$

También se incluye una parte del ejerccio *bonus*. Para esta parte, se crea la clase hija TiendaOnline_2: 

**Clase**: TiendaOnline_2(TiendaOnline)

**Atributos**:
- clientes: Un atributo para llevar un registro de los clientes de la tienda en forma de diccionario de diccionarios.

**Métodos**:

- `agregar_cliente(self, nombre, email)`: 

    Agrega un cliente al diccionario de clientes con su nombre y correo electrónico

- `ver_clientes(self)`

    Muestra la lista de clientes registrados con sus nombres y correos electrónicos

- `realizar_compra(self)`:

     Permite a un cliente realizar una compra seleccionando productos del inventario. Debe interactuar con el cliente para seleccionar productos y calcular el costo total de la compra.

    
## Final exercise Module 1 Adalab Data Analytics Bootcamp 

This repository contains the evaluation exercise for Module 1 (Basic Python) from the Adalab Data Analytics Bootcamp. It also includes a draft file that collects tests used during the development process.

The exercise consists of creating the TiendaOnline class with the following structure:

**Class**: TiendaOnline

**Attributes**:

- inventario: List of dictionaries with products (name, price, quantity).
- ventas_totales: float, initialized to 0.

**Methods**:

- `agregar_producto(name, price, quantity)`

    If the product exists, update its quantity.
    If not, add a new product.

- `ver_inventario()`

    Displays all inventory products.

- `buscar_producto(name)`

    Search for a product by name and display its details if found.

- `actualizar_stock(name, quantity)`

    Updates the quantity of an existing product.
    Displays a message if the product is not found.

- `eliminar_producto(name)`

    Deletes a product by name if it exists.
    Displays a message if not found.

- `calcular_valor_inventario()`

    Calculates the sum of products in inventory as:

    $$
    \sum Inventory_{total} = price*quantity
    $$

    A part of the bonus exercise is also included. For this part, the child class TiendaOnline_2 is created:

**Class**: TiendaOnline_2(TiendaOnline)

**Attributes**:

- clientes: An attribute to keep track of store customers in the form of a dictionary of dictionaries.

**Methods**:

- agregar_cliente(self, nombre, email):

    Adds a customer to the clientes dictionary, including their name and email.

- ver_clientes(self):

    Displays the list of registered customers with their names and email addresses.

- realizar_compra(self):

    Allows to make a purchase by selecting products from the inventory. It should interact with the customer to select products and calculate the total purchase cost.