======================================================================
PROYECTO: Formulario de Pedido de Agroinsumos
ARCHIVO PRINCIPAL: AgroPedidos.html
DESCRIPCIÓN: Maqueta de una aplicación tipo 'ventana' que contiene un iframe para un formulario de pedido de agroinsumos.
======================================================================

### 1. Propósito

Este documento describe la configuración y los detalles necesarios para el despliegue del archivo `AgroPedidos.html` en Netlify.

### 2. Archivos a Desplegar

* **AgroPedidos.html**: El único archivo necesario. Contiene la estructura, estilos CSS (incrustados en la etiqueta `<style>`), y el contenido principal.

### 3. Configuración de Netlify

**Configuración Básica:**

* **Directorio de Publicación (Publish directory):** Dejar en blanco o configurar como `./` (raíz). Dado que solo hay un archivo HTML, Netlify lo detectará automáticamente.
* **Comando de Construcción (Build command):** No se requiere ningún comando de construcción (dejar en blanco), ya que es un archivo HTML estático puro sin preprocesadores ni frameworks.

**Detalles del Despliegue:**

* **Dominio Principal:** El archivo `AgroPedidos.html` será el archivo raíz (index) del sitio. Si se desea que sea la página de inicio, asegúrate de que Netlify lo reconozca como tal, o re-nómbralo a `index.html` antes de subirlo.
    * **Recomendación:** Renombrar `AgroPedidos.html` a **`index.html`** para asegurar que se cargue automáticamente al acceder a la URL principal del sitio de Netlify.

### 4. Detalles del Iframe (Contenido Incrustado)

El formulario está incrustado usando un `<iframe>`.

* **URL del Formulario:** `https://tally.so/r/3E4DKl`
* **Nota:** Este enlace debe estar operativo para que el formulario se muestre correctamente dentro de la ventana de la aplicación simulada.

### 5. Variables de Entorno y Configuración Adicional

* No se requieren variables de entorno.
* No se requiere configuración de funciones Serverless (Functions).
* No se requiere redireccionamiento (`_redirects`) a menos que se necesite una URL amigable específica.
