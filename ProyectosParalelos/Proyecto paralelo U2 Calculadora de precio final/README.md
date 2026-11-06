# Calculadora de Precio Final con IVA y Descuentos

Aplicación de escritorio desarrollada en Python utilizando la librería `Tkinter` (y su módulo temático `ttk`). Esta herramienta permite calcular el desglose completo del precio final de un producto a partir de su precio base, aplicando diferentes tipos de IVA y porcentajes de descuento.

## Características principales

* **Interfaz Gráfica Amigable:** Interfaz limpia estructurada con `ttk.Frame`, `ttk.Combobox`, `ttk.Spinbox` y adaptada para una visualización clara a 360x400 píxeles.
* **Tipos de IVA personalizables:** Permite seleccionar entre IVA General (21%), Reducido (10%), Superreducido (4%) y Exento (0%).
* **Flexibilidad en el precio:** Opción para indicar si el precio introducido por el usuario ya incluye el IVA o no mediante un `Checkbutton`.
* **Cálculo de Descuentos:** Integración de un selector de descuentos de 0% a 100% en incrementos del 5%.
* **Desglose Detallado:** Al calcular, el sistema muestra un "ticket" alineado en columnas con fuente monoespaciada (`TkFixedFont`) que incluye:
  * Base imponible
  * Descuento aplicado (importe y porcentaje)
  * Base con descuento
  * Importe del IVA
  * TOTAL (formateado a 2 decimales con el símbolo €)
* **Validación de Datos y Manejo de Errores:** Filtra entradas no válidas (letras, valores negativos, o valores nulos como `nan` e `inf`) mostrando alertas descriptivas en color rojo.

## Tecnologías utilizadas

* **Lenguaje:** Python 3.x
* **Librerías:** 
  * `tkinter` (Librería estándar de Python para interfaces gráficas)
  * `math` (Para validaciones matemáticas avanzadas)

## Instrucciones de Uso

1. Asegúrate de tener instalado Python 3 en tu sistema. No se requieren librerías externas.
2. Descarga o clona este repositorio.
3. Ejecuta el archivo principal desde la terminal o tu IDE favorito:
   ```bash
   python nombre_del_archivo.py
   ```
4. En la ventana de la aplicación:
   * Selecciona el **Tipo de IVA**.
   * Introduce el **Precio en euros** (se admiten puntos y comas como separador decimal).
   * Selecciona el **Porcentaje de descuento**.
   * Marca la casilla si el precio original ya tiene el IVA incluido.
   * Pulsa **Calcular** para ver el desglose o **Limpiar** para reiniciar el formulario.

## Estructura del Código

El proyecto está diseñado bajo el paradigma de Programación Orientada a Objetos (POO). Toda la lógica visual y matemática está encapsulada dentro de la clase `Ventana`, lo que facilita la escalabilidad, la lectura del código y el mantenimiento de la aplicación.
