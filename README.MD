# StoreApp Analyst

Este proyecto es una aplicación diseñada para analizar datos provenientes de una API de una tienda en línea. Utiliza herramientas de análisis de datos como Pandas, Matplotlib y Seaborn para procesar y visualizar la información sobre productos, órdenes y categorías.

---

## 📋 **Características del Proyecto**

1. **Análisis de Productos**:

    - Distribución de precios.
    - Productos más caros por categoría.
    - Precio promedio por categoría.
    - Relación entre precio y calificación promedio.

2. **Análisis de Órdenes**:

    - Cantidad de órdenes por estado (`pending`, `completed`, etc.).
    - Tendencia de órdenes por día o mes.

3. **Visualización de Datos**:

    - Gráficos de barras, líneas, dispersión y pastel.
    - Análisis de datos clave utilizando Python y librerías de visualización como Matplotlib y Seaborn.

4. **Interacción con la API**:
    - Uso de `requests` para obtener datos desde una API.
    - Manejo de datos en formato JSON para convertirlos en DataFrames de Pandas.

---

## 🚀 **Cómo Ejecutar el Proyecto**

### **Requisitos Previos**

-   Python 3.8 o superior.
-   Las siguientes bibliotecas de Python instaladas:
    -   `pandas`
    -   `matplotlib`
    -   `seaborn`
    -   `requests`

Instálalas con el siguiente comando:

```bash
    pip install pandas matplotlib seaborn requests
```

## 🛠️ Cómo Probar la API en Postman

1. **Importa la Colección en Postman**:

    - Abre Postman y selecciona la opción de "Importar".
    - Ingresa las siguientes rutas de ejemplo para probar la API:
        - **Productos**: `GET /products` - Obtiene todos los productos.
        - **Categorías**: `GET /categories` - Lista las categorías disponibles.
        - **Órdenes**: `GET /orders` - Recupera el estado de todas las órdenes.

2. **Añade el Token de Autenticación**:

    - En cada solicitud, ve a la pestaña `Authorization` y selecciona `Bearer Token`.
    - Copia y pega tu token JWT en el campo correspondiente.

3. **Prueba los Endpoints**:

    - Envía las solicitudes para verificar que la API funcione correctamente.
    - Algunos endpoints importantes que puedes probar:
        - **`GET /products`**: Obtiene la lista de productos.
        - **`GET /products/{id}`**: Obtiene los detalles de un producto por su ID.
        - **`GET /categories`**: Lista todas las categorías disponibles.
        - **`GET /orders`**: Recupera todas las órdenes y su estado.

4. **Valida la Respuesta**:
    - Verifica que los datos devueltos por la API coincidan con lo esperado.
    - Por ejemplo, para el endpoint `/products`, deberías obtener una lista de productos con campos como `id`, `name`, `price`, etc.

---

## 📊 Ejemplo de Visualizaciones Generadas

1. **Distribución de Precios**:
   ![Distribución de Precios](./images/price_distribution.png)

2. **Precio Promedio por Categoría**:
   ![Precio Promedio por Categoría](./images/avg_price_by_category.png)

3. **Órdenes por Estado**:
   ![Órdenes por Estado](./images/orders_by_status.png)

4. **Relación Precio vs Calificación**:
   ![Relación Precio vs Calificación](./images/price_vs_rating.png)

---

## 📂 Estructura del Proyecto

    StoreApp-Analyst/
    ├── analyzer.py         # Código principal para análisis de datos.
    ├── requirements.txt    # Lista de dependencias.
    ├── images/             # Carpeta donde se guardan los gráficos generados.
    └── README.md           # Archivo de documentación del proyecto.

---

## 💡 Características Futuras

-   Agregar gráficos interactivos.
-   Implementar un frontend para explorar los análisis sin necesidad de ejecutar Python.
-   Soporte para más endpoints de API, como carrito de compras.

---

## 👨‍💻 Contribución

Las contribuciones son bienvenidas. Si deseas mejorar el proyecto, envía un pull request con tus cambios. Para ideas o reportes de bugs, utiliza la sección de "Issues".

---

## 📝 Licencia

Este proyecto está bajo la Licencia MIT. Consulta el archivo `LICENSE` para más detalles.
