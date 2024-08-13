Aplicación de movimiento del cursor del mouse usando YOLOv8 y Android

Paso 1 (Entrenar y exportar el modelo de detección de objetos):

Entrenar el modelo yolov8 en un conjunto de datos personalizado y expórtalo en formato .tflite. (Consulta train_export_yolov8_model.ipynb)

Paso 2 (Configuración de la aplicación de detección de objetos para Android):

Abre la carpeta android_app.

Colocar el modelo .tflite y el archivo de etiquetas .txt dentro de la carpeta assets. Puede encontrar la carpeta assets en esta ubicación: <b> android_app\android_app\app\src\main\assets</b>

Cambie los caminos del modelo y del archivo de etiquetas en el archivo Constants.kt. Puede encontrar Constants.kt en esta ubicación: <b>android_app\android_app\app\src\main\java\com\vis2ai\yolov8tflite</b>

En res/values/string reemplazar con la IP local de la PC a controlar. Se utiliza puerto 5005.

Paso 3 (Obtención de la ubicación detectada del mouse)

Utilice el notebook mouse_cursor_controller.ipynb para habilitar el control del mouse vía WiFi

Créditos
Este proyecto incluye el código de la aplicación de Android del siguiente repositorio:
(https://github.com/surendramaran/YOLOv8-TfLite-Object-Detector)

Video disponible:
Consulte el video para entender el código: https://youtu.be/dl7rCmvIyiI

Gracias a (https://github.com/surendramaran) por su contribución.