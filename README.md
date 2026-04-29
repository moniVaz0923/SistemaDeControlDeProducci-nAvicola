Sistema de Gestión Avícola
Este proyecto es una aplicación desarrollada en Python diseñada para supervisar y optimizar los datos críticos de producción en granjas avícolas de pollos parrilleros. Aunque el desarrollo inicial se centró en las necesidades de Granja Pando, la arquitectura está preparada para escalar a múltiples empresas, comenzando la expansión con ARGEAVE.

🚀 Funcionalidades Principales
Control de Mortandad: Registro detallado y seguimiento de las bajas en los lotes.

Gestión de Alimento: Supervisión de los niveles de alimento ingresado y control del consumo diario.

Sincronización Híbrida: Capacidad de trabajar con bases de datos locales (SQLite) y sincronizar la información con la nube (MySQL) para asegurar la disponibilidad de los datos.

Gestión Multi-empresa: Estructura modular preparada para integrarse a diferentes entornos corporativos.

🛠️ Tecnologías Utilizadas
Lenguaje: Python 3.x

Base de Datos Local: SQLite (para operación offline)

Base de Datos Cloud: MySQL

Librerías principales: (Aquí puedes listar las que uses, ej: mysql-connector-python, pandas, etc.)

📂 Estructura del Proyecto
main_app.py: Punto de entrada principal de la aplicación.

db_cloud.py / db_local.py: Módulos de conexión y gestión de las bases de datos.

sync.py: Lógica encargada de la persistencia y subida de datos locales a la nube.

config.py: Archivo de configuración para variables de entorno y credenciales.

⚙️ Instalación y Configuración
Clonar el repositorio:

Bash
git clone (https://github.com/moniVaz0923/SistemaDeControlDeProducci-nAvicola.git)
Instalar dependencias:

Bash
pip install -r requirements.txt
Configurar el archivo config.py con las credenciales de la base de datos MySQL en la nube.

Ejecutar la aplicación:

Bash
python main_app.py
