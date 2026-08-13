<h1 align="center">BioTiendApp</h1>
<p align="center">
  Proyecto final en Java para el módulo de <strong>Programación Orientada a Objetos</strong>.<br>
  Sistema de gestión para una tienda de alimentos orgánicos.
</p>

---

## Tecnologías utilizadas

<ul>
  <li><strong>Java 21</strong></li>
  <li>Herramientas utilizadas:</li>
  <ul>
    <li><img src="https://img.icons8.com/color/20/intellij-idea.png"/> IntelliJ IDEA (IDE)</li>
    <li><img src="https://img.icons8.com/color/20/visual-studio-code-2019.png"/> Visual Studio Code (Editor de código)</li>
  </ul>
</ul>

---

## Descripción

BioTiendApp es una aplicación de consola que permite la <strong>gestión de productos y proveedores</strong> para una tienda de alimentos orgánicos.

### Funciones principales:

- Registrar nuevos productos (nombre, tipo, proveedor, etc.)
- Registrar y consultar proveedores (locales e internacionales)
- Ver listados de productos y proveedores registrados
- Menú interactivo por consola

### Arquitectura del proyecto

```
BioTiendApp
├── model
│   ├── product
│   │   ├── Fruit.java
│   │   ├── Vegetable.java
│   │   └── OrganicProduct.java
│   └── supplier
│       ├── Supplier.java
│       ├── LocalSupplier.java
│       └── InternationalSupplier.java
├── services
│   ├── SupplierService.java
│   └── OrganicStoreService.java
├── ui
│   ├── GeneralMenu.java
│   ├── ProductUi.java
│   ├── SupplierUi.java
│   └── ConsoleUtils.java
└── App.java (Clase principal)
```

---

## Flujo de trabajo

> **Nota importante:**
> Para poder registrar un producto correctamente, primero se debe registrar un proveedor.
> Esto se debe a que cada producto requiere un proveedor asociado al momento de su creación.

Pasos recomendados:

1. Registrar uno o más proveedores (local o internacional).
2. Crear los productos, seleccionando un proveedor existente.
3. Consultar o gestionar los elementos registrados desde el menú principal.

---

## Cómo ejecutar

<ol>
  <li><strong>Clonar el repositorio:</strong>
    <pre><code>git clone https://github.com/themisael2004/BioTiendApp.git</code></pre>
    <pre><code>cd BioTiendApp</code></pre>
    <em>(Asegúrate de navegar al directorio raíz del proyecto después de clonarlo.)</em>
  </li>
  <li><strong>Compilar el proyecto desde consola:</strong>
    <br>
    <em>(Este comando compilará todos los archivos <code>.java</code> dentro de la carpeta <code>src</code> y sus subdirectorios, colocando los archivos <code>.class</code> resultantes en la carpeta <code>bin</code>.)</em>
    <pre><code>find src -name "*.java" -print0 | xargs -0 javac -d bin</code></pre>
  </li>
  <li><strong>Ejecutar la clase principal:</strong>
    <br>
    <em>(Este comando ejecutará la aplicación, indicando a la Java Virtual Machine (JVM) que busque las clases compiladas en el directorio <code>bin</code>.)</em>
    <pre><code>java -cp bin App</code></pre>
  </li>
</ol>

---

## Autores

<ul>
  <li><strong>Vanessa Gabriela Arévalo Elías</strong></li>
  <li><strong>Lizzie Nicole Beltrán Peña</strong></li>
  <li><strong>Cesia Mariena Alfaro Hernández</strong></li>
  <li><strong>Bryan Misael Sánchez Ramírez</strong></li>
</ul>
