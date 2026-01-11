# readme-el-buen-taco

# El Buen Taco

Sistema de gestión de pedidos para restaurantes que permite a los clientes realizar pedidos de manera remota y a los administradores gestionar tanto pedidos como clientes de forma eficiente.

## Descripción

El Buen Taco es una aplicación web diseñada para modernizar la experiencia de pedidos en restaurantes. Los clientes pueden explorar el menú y realizar pedidos desde la comodidad de su dispositivo, mientras que el personal administrativo cuenta con herramientas completas para supervisar y administrar todas las operaciones del negocio.

## Características Principales

### Para Clientes
- Navegación intuitiva del menú del restaurante
- Sistema de autenticación seguro (login y registro)
- Realización de pedidos personalizados con especificaciones de alimentos
- Selección de hora de entrega y método de pago
- Panel "Mis Pedidos" para seguimiento de pedidos activos
- Interfaz responsiva y fácil de usar con diseño atractivo

### Para Administradores
- Panel de control administrativo completo
- Gestión de pedidos (visualizar, actualizar estado, cancelar)
- Administración de clientes (registro, consulta, modificación)
- Soporte para clientes tipo "Persona Física" y otros tipos
- Gestión del menú y productos
- Sistema de autenticación diferenciado para administradores

## Tecnologías Utilizadas

- **Frontend**: HTML (44.3%), CSS (14.4%), JavaScript
- **Backend**: C# (41.3%) / ASP.NET
- **Base de datos**: SQL Server
- **Framework**: .NET Framework/Core

## Instalación

1. Clona el repositorio:
```bash
git clone https://github.com/LuisHV935/El-Buen-Taco.git
cd El-Buen-Taco
```

2. Abre el proyecto en Visual Studio (2019 o superior recomendado)

3. Restaura los paquetes NuGet:
```bash
dotnet restore
```

4. Configura la cadena de conexión a la base de datos en `Web.config` o `appsettings.json`:
```xml
<connectionStrings>
  <add name="DefaultConnection" 
       connectionString="Server=tu_servidor;Database=ElBuenTaco;Trusted_Connection=True;" 
       providerName="System.Data.SqlClient" />
</connectionStrings>
```

5. Ejecuta las migraciones de la base de datos:
```bash
Update-Database
```

6. Ejecuta la aplicación presionando F5 en Visual Studio o mediante:
```bash
dotnet run
```

## Configuración

### Requisitos Previos
- Visual Studio 2019 o superior
- .NET Framework 4.7+ o .NET Core 3.1+
- SQL Server 2016 o superior (o SQL Server Express)
- IIS (para despliegue en producción)

### Configuración de la Base de Datos
1. Crea una base de datos llamada `ElBuenTaco` en SQL Server
2. Actualiza la cadena de conexión en el archivo de configuración
3. Ejecuta las migraciones para crear las tablas necesarias

### Credenciales de Administrador
Después de la primera ejecución, puedes acceder con las credenciales por defecto (si están configuradas en el seed) o crear un usuario administrador desde la base de datos.

## Uso

### Acceso como Cliente
1. Accede a la aplicación desde tu navegador
2. Si no tienes cuenta, haz clic en "Crear cuenta" y completa el formulario de registro:
   - Email
   - Contraseña
   - Nombre completo
   - Teléfono
   - Tipo de cliente (Persona Física, etc.)
3. Inicia sesión con tus credenciales
4. En el panel "Mis Pedidos", haz clic en "Nuevo pedido" o "Hacer pedido"
5. Especifica los alimentos que deseas (ej. "2 tacos pastor, 1 agua")
6. Selecciona la hora de entrega y método de pago
7. Envía tu pedido y espera la confirmación

### Acceso como Administrador
1. Inicia sesión con credenciales de administrador
2. Accede al panel de control administrativo
3. Gestiona pedidos, clientes y productos según sea necesario
4. Actualiza el estado de los pedidos en tiempo real

## Contribuciones

Las contribuciones son bienvenidas. Si deseas contribuir:

1. Haz fork del proyecto
2. Crea una rama para tu feature (`git checkout -b feature/NuevaCaracteristica`)
3. Realiza tus cambios y haz commit (`git commit -m 'Añade nueva característica'`)
4. Push a la rama (`git push origin feature/NuevaCaracteristica`)
5. Abre un Pull Request

## Licencia

Este proyecto está bajo la Licencia [especifica tu licencia]. Ver el archivo `LICENSE` para más detalles.

## Autor

**Luis HV**
- GitHub: [@LuisHV935](https://github.com/LuisHV935)

## Contacto

Si tienes alguna pregunta o sugerencia, no dudes en abrir un issue en el repositorio.

## Capturas de Pantalla

### Pantalla de Inicio de Sesión
![Login](screenshots/login.png)
*Interfaz de acceso a la cuenta con diseño atractivo de fondo con tacos*

### Pantalla de Registro
![Registro](screenshots/registro.png)
*Formulario completo de registro con validación de datos*

### Panel de Bienvenida - Mis Pedidos
![Mis Pedidos](screenshots/mis-pedidos.png)
*Vista principal donde los clientes pueden ver sus pedidos y crear nuevos*

### Formulario de Nuevo Pedido
![Nuevo Pedido](screenshots/nuevo-pedido.png)
*Interfaz para crear pedidos personalizados con selección de hora y método de pago*
