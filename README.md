## Uso de Bootstrap

Este portafolio está diseñado utilizando **Bootstrap 5**, un potente framework CSS que facilita la creación de sitios web responsivos y atractivos. A continuación, se describen con más detalle las características y componentes de Bootstrap implementados en este proyecto:

### 1. **Sistema de Rejillas (Grid System)**
   - Utilicé el sistema de rejillas de Bootstrap para organizar el contenido en una estructura de columnas flexibles y adaptativas. La clase `container` se utiliza para envolver todo el contenido, proporcionando un diseño con márgenes y un ancho fijo en pantallas grandes.
   - Las clases `row` y `col` permiten dividir el contenido en filas y columnas, respetando las diferentes resoluciones de pantalla.
     - **Ejemplo:**
       ```html
       <div class="row gx-5 align-items-center">
           <div class="col-xxl-5">
               <!-- Contenido -->
           </div>
           <div class="col-xxl-7">
               <!-- Contenido -->
           </div>
       </div>
       ```
     - Esto asegura que el contenido se reorganicé adecuadamente en dispositivos de diferentes tamaños, como móviles, tabletas y escritorios.

### 2. **Navbar (Barra de Navegación)**
   - La barra de navegación está implementada usando el componente `navbar` de Bootstrap, con clases como `navbar-expand-lg` que hacen que la barra de navegación se contraiga en pantallas pequeñas y se expanda en pantallas más grandes.
   - El botón de menú desplegable (hamburguesa) se habilita con la clase `navbar-toggler` junto con `data-bs-toggle="collapse"`, lo que hace que el menú se oculte o se muestre al hacer clic en dispositivos móviles.
   - **Ejemplo:**
     ```html
     <nav class="navbar navbar-expand-lg navbar-light bg-white py-3">
         <button class="navbar-toggler" type="button" data-bs-toggle="collapse" data-bs-target="#navbarSupportedContent">
             <span class="navbar-toggler-icon"></span>
         </button>
         <div class="collapse navbar-collapse" id="navbarSupportedContent">
             <ul class="navbar-nav ms-auto mb-2 mb-lg-0">
                 <li class="nav-item"><a class="nav-link" href="#projects">Proyectos</a></li>
                 <li class="nav-item"><a class="nav-link" href="#skills">Habilidades</a></li>
                 <li class="nav-item"><a class="nav-link" href="#contact">Contacto</a></li>
             </ul>
         </div>
     </nav>
     ```
   - Esto asegura una experiencia de navegación fluida en dispositivos de todos los tamaños.

### 3. **Cards (Tarjetas) para los Proyectos**
   - Para los proyectos, se usaron **Cards** de Bootstrap, lo que proporciona un diseño limpio y consistente para presentar cada uno de ellos. Dentro de cada tarjeta, se incluye una imagen, título y descripción, organizados con `d-flex` y `align-items-center` para asegurar una alineación adecuada.
   - Se utilizó `shadow` y `rounded-4` para agregar un efecto de sombra y bordes redondeados, respectivamente.
   - **Ejemplo:**
     ```html
     <div class="col-md-6 mb-4">
         <div class="card overflow-hidden shadow rounded-4 border-0">
             <div class="card-body p-0">
                 <div class="d-flex align-items-center">
                     <div class="p-4">
                         <h2 class="fw-bolder">Odoo</h2>
                         <p>Descripción del proyecto...</p>
                     </div>
                     <img src="assets/proyecto_1.png" alt="Odoo" class="img-proyecto1" />
                 </div>
             </div>
         </div>
     </div>
     ```

### 4. **Formularios**
   - El formulario de contacto utiliza las clases de **Formulario** de Bootstrap como `form-floating`, que proporciona un diseño más limpio para los campos de entrada, y `form-control`, que aplica los estilos predeterminados de Bootstrap para los campos de texto.
   - Se añadió validación de formularios con las clases de Bootstrap, como `invalid-feedback`, para mostrar mensajes de error si el usuario no completa un campo correctamente.
   - **Ejemplo:**
     ```html
     <form id="contactForm">
         <div class="form-floating mb-3">
             <input class="form-control" id="name" type="text" placeholder="Enter your name..." />
             <label for="name">Full name</label>
         </div>
         <button class="btn btn-primary btn-lg" type="submit">Submit</button>
     </form>
     ```

### 5. **Botones**
   - Se utilizaron botones con clases de Bootstrap como `btn` y `btn-primary` para estilizar los botones del formulario y los enlaces, asegurando que tengan una apariencia coherente y atractiva.
   - **Ejemplo:**
     ```html
     <button class="btn btn-primary btn-lg" type="submit">Enviar</button>
     ```

### 6. **Iconos de Bootstrap**
   - Se integraron **iconos de Bootstrap** (Bootstrap Icons) en la barra de navegación y en las secciones para dar un toque visual y facilitar la navegación del usuario.
   - Utilicé clases como `bi bi-house-door` y `bi bi-envelope` para los íconos de "inicio" y "correo electrónico", respectivamente.
   - **Ejemplo:**
     ```html
     <a class="text-white me-3" href="#home"><i class="bi bi-house-door"></i></a>
     ```

### 7. **Diseño Responsivo y Flexibilidad**
   - Gracias al uso de clases como `d-flex`, `justify-content-center`, `align-items-center`, y `container-fluid`, todo el contenido se adapta de forma fluida a diferentes tamaños de pantalla, desde dispositivos móviles hasta pantallas de escritorio.
   - Las clases como `mb-3` y `px-5` se utilizan para ajustar los márgenes y los rellenos para una mejor distribución del contenido.

### 8. **Efectos Visuales y Personalización de Estilo**
   - A través de clases como `bg-gradient-primary-to-secondary`, se aplicaron degradados personalizados a varias secciones del sitio, creando un estilo visual atractivo.
   - La personalización de los colores y el uso de tipografía a través de Google Fonts (como `Plus Jakarta Sans`) ayudaron a definir un estilo único.

### 9. **Popper.js y Bootstrap JS**
   - Para habilitar los elementos interactivos, como los menús desplegables de la barra de navegación en dispositivos móviles, se integraron **Popper.js** y **Bootstrap JS**. Estas bibliotecas permiten la correcta visualización y funcionalidad de los elementos dinámicos, como el colapso del menú.

   - **Ejemplo:**
     ```html
     <script src="https://cdn.jsdelivr.net/npm/@popperjs/core@2.11.6/dist/umd/popper.min.js"></script>
     <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.0-beta1/dist/js/bootstrap.min.js"></script>
     ```

