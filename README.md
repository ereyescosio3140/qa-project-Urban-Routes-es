Automatización de Pruebas de IU para Urban Routes

Este proyecto implementa pruebas automatizadas para la interfaz de usuario de una aplicación de Urban Routes. Las pruebas se han diseñado utilizando Selenium y están estructuradas para ser dinámicas y adaptables.

Estructura del Proyecto

helpers.py: Contiene métodos auxiliares, como get_phone_code, que recupera partes específicas de datos, como el código de un número de teléfono.
data.py: Archivo para almacenar datos dinámicos utilizados en las pruebas, como direcciones, números de teléfono y códigos de tarjeta.
urban_routes_page.py: Implementa los localizadores y métodos para interactuar con los elementos de la página.
main.py: Contiene las pruebas unitarias que validan la funcionalidad de la aplicación.
Instalación

Clona este repositorio:
git clone https://github.com/usuario/urban-routes-automation.git
cd urban-routes-automation
Instala los requisitos:
pip install -r requirements.txt
Asegúrate de tener Google Chrome y el driver de Chrome instalados.
Configuración

Configura la URL y los datos dinámicos en data.py:
urban_routes_url = "https://urbanroutes.example.com"
address_from = "123 Main St"
address_to = "456 Elm St"
phone_number = "+1 123 123 12 12"
card_code = "123"
Verifica que el archivo data.py contiene la información necesaria para las pruebas.
Ejecución de las Pruebas

Ejecuta las pruebas desde el archivo main.py:
python main.py
Las pruebas cubrirán los siguientes casos:
Validación de direcciones de origen y destino.
Selección de tarifas y opciones adicionales.
Envío de mensajes.
Verificación de interacciones con botones y cuadros de texto.
Detalles Técnicos

Localizadores: Se han mejorado para ser compatibles con cualquier navegador utilizando CSS_SELECTOR y XPATH.
Datos Dinámicos: Se obtienen desde data.py para garantizar flexibilidad y evitar información estática.
Pruebas Unitarias: Se utiliza unittest para estructurar y ejecutar las pruebas.
Notas

Los cambios realizados están resaltados con comentarios en los archivos correspondientes.
Cada método de prueba utiliza un assert para verificar si el resultado es el esperado.
Próximos Pasos

Asegúrate de que las pruebas funcionan en múltiples navegadores.
Considera implementar pruebas adicionales para validar casos extremos o negativos.
Recursos

Documentación de Selenium
Unittest en Python
