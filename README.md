# Informe Final del Proyecto: Pruebas de la Aplicación Móvil **Urban.Lunch** para Android

## **Descripción del Proyecto**
La aplicación móvil **Urban.Lunch** permite a los usuarios pedir comidas de diferentes restaurantes y recogerlas en puntos designados. Este proyecto se enfocó en probar la primera versión de la aplicación desarrollada para Android, validando funcionalidad, experiencia de usuario y desempeño.

---

## **Objetivos**
1. Analizar los requisitos funcionales y no funcionales de la aplicación.
2. Crear una lista de comprobación para probar la funcionalidad seleccionada.
3. Probar la aplicación utilizando un emulador de **Android Studio** y/o un dispositivo físico Android.
4. Documentar errores (bugs) en **Jira** y proporcionar un informe sobre el estado de la aplicación.

---

## **Requisitos Probados**
Se centraron las pruebas en la funcionalidad relacionada con **realizar un pedido y gestionarlo hasta la recogida**, incluyendo:
1. Navegación por la lista de restaurantes.
2. Selección de un restaurante y su menú.
3. Proceso de pedido (selección de platos, pago y confirmación).
4. Notificaciones sobre el estado del pedido (e.g., "Pedido confirmado", "En preparación", "Listo para recoger").
5. Gestión de puntos de recogida.

---

## **Lista de Comprobación**

### **1. Navegación por la Lista de Restaurantes**
#### **Casos Positivos**
1. La lista de restaurantes se carga correctamente al abrir la aplicación.
2. Los restaurantes aparecen ordenados según la distancia al usuario.
3. Las imágenes y descripciones de los restaurantes se cargan sin errores.
4. La búsqueda de un restaurante por nombre filtra los resultados correctamente.

#### **Casos Negativos**
1. Verificar que se muestra un mensaje adecuado al no haber conexión a internet.
2. Comprobar el comportamiento al introducir caracteres inválidos en el campo de búsqueda.
3. Simular la carga de restaurantes con la ubicación desactivada.

---

### **2. Selección de Restaurante y Menú**
#### **Casos Positivos**
1. El menú de cada restaurante se carga al seleccionarlo.
2. Al seleccionar un platillo, se muestran los detalles (ingredientes, precio, opciones adicionales).
3. El botón "Agregar al carrito" funciona correctamente.

#### **Casos Negativos**
1. Intentar agregar un platillo al carrito sin seleccionar opciones obligatorias (e.g., tamaño, bebida).
2. Comprobar el mensaje al intentar acceder a un restaurante cerrado.
3. Simular la pérdida de conexión durante la carga del menú.

---

### **3. Proceso de Pedido y Confirmación**
#### **Casos Positivos**
1. Al confirmar el pedido, se muestra un resumen con los platos seleccionados y el punto de recogida.
2. Los métodos de pago disponibles funcionan correctamente (e.g., tarjeta, PayPal).
3. Se generan notificaciones al cambiar el estado del pedido.

#### **Casos Negativos**
1. Intentar realizar un pedido sin seleccionar un punto de recogida.
2. Verificar el comportamiento al introducir datos de pago inválidos.
3. Simular la pérdida de conexión durante el proceso de pago.

---

### **4. Gestión de Puntos de Recogida**
#### **Casos Positivos**
1. Los puntos de recogida cercanos se muestran en un mapa.
2. El usuario puede seleccionar un punto de recogida y verlo en el resumen del pedido.
3. Cambiar el punto de recogida antes de confirmar actualiza el resumen.

#### **Casos Negativos**
1. Verificar el comportamiento si no hay puntos de recogida cercanos disponibles.
2. Intentar seleccionar un punto de recogida deshabilitado o fuera de horario.
3. Simular fallos de geolocalización al cargar puntos de recogida.

---

## **Resultados de las Pruebas**

### **Herramientas Utilizadas**
- **Android Studio:** Para pruebas en emulador.
- **Dispositivo Android:** Pruebas en un entorno físico real.
- **Jira:** Para documentar y rastrear errores detectados.

### **Resumen de Resultados**
1. **Total de casos probados:** 24
2. **Casos exitosos:** 19
3. **Errores detectados:** 5

---

## **Errores Detectados**
1. **Navegación:** No se muestra un mensaje claro cuando no hay conexión a internet.
2. **Menú:** El botón "Agregar al carrito" no responde si no se seleccionan opciones obligatorias.
3. **Pedido:** Las notificaciones de estado no se generan en algunos casos.
4. **Puntos de Recogida:** Los puntos deshabilitados no se diferencian visualmente de los habilitados.
5. **General:** La aplicación se bloquea si se pierde la conexión durante el pago.

---

## **Conclusión**
La funcionalidad principal de **Urban.Lunch** está operativa y cumple con la mayoría de los casos probados. Sin embargo, se identificaron errores que podrían impactar negativamente la experiencia del usuario en escenarios clave, como la gestión de pedidos y puntos de recogida.

---

## **Recomendaciones**
1. Implementar un mejor manejo de errores para situaciones como falta de conexión o fallos de geolocalización.
2. Asegurar que las notificaciones de estado del pedido se generen consistentemente.
3. Mejorar la diferenciación visual de puntos de recogida habilitados y deshabilitados.
4. Realizar una ronda adicional de pruebas tras implementar las correcciones.

---

**Equipo QA de Urban.Lunch**  

**Enlaces Relacionados:**
- **Lista de Comprobación:** [[Ver Inform Final](https://drive.google.com/drive/folders/1-Pib6bJray0gx1XCI2H5y4Kfig6NJ-p2?usp=sharing)](#)
