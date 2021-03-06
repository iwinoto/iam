---

copyright:

  years: 2015, 2018
lastupdated: "2018-05-02"

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:new_window: target="_blank"}

# Asignación de acceso de usuario
{: #assignaccess}

Puede asignar acceso a los usuarios a medida que los invita, asignando permisos de infraestructura, políticas y roles de Cloud Foundry. Según las opciones de acceso que esté autorizado a gestionar, puede invitar y proporcionar acceso a usuarios de la cuenta, organización, espacio e instancias de servicio. En las secciones siguientes se describen los tres tipos de acceso que se pueden asignar a un usuario invitado.
{:shortdesc}

## Servicios habilitados para identificación y acceso

Puede asignar una política de servicio individual cuando invite a un nuevo usuario. Cuando el usuario acepte la invitación, podrá añadir políticas de servicio adicionales.

1. Desde la pantalla **Invitar a usuarios**, amplíe la sección **Servicios habilitados para Identity and Access**.
2. Seleccione un servicio.
3. Seleccione **Todas las regiones actuales** o una región específica.
4. Seleccione **Todas las instancias de servicio actuales** o seleccione una instancia de servicio específica.
5. Seleccione un rol para definir el ámbito del acceso para la política.
6. De forma opcional, puede seleccionar **Añadir rol** para especificar otro rol para la política.

Para obtener más información sobre los roles al configurar políticas de servicio, consulte [Roles y políticas de gestión de acceso e identidad](/docs/iam/users_roles.html#iamusermanpol).

## Acceso de Cloud Foundry

Cuando invita a nuevos usuarios, puede elegir añadirlos a una organización en la cuenta. Si añade los usuarios a una organización, puede asignar al usuario un rol de organización. A continuación, seleccione proporcionar acceso al usuario invitado a uno o a todos los espacios de la organización seleccionada con un rol de espacio asignado.

1. Desde la pantalla **Invitar usuarios**, expanda la sección **Acceso de Cloud Foundry**.
2. Seleccione una organización en la que añadir al usuario.
3. Seleccione un rol de organización para definir el nivel de acceso a la organización seleccionada.
4. Opcional: Seleccione **Añadir rol** para especificar un rol adicional.
5. Seleccione **Todas las regiones actuales** o una región específica.
6. Seleccione **Todos los espacios actuales** o un espacio específico.
7. Seleccione un rol de espacio para definir el nivel de acceso a los espacios seleccionados.
8. De forma opcional, puede seleccionar **Añadir rol** para especificar otro rol para la política.

Para obtener más información sobre los roles, consulte [Roles de Cloud Foundry](/docs/iam/users_roles.html#cfroles).

**Nota**: Es posible añadir un rol de Cloud Foundry utilizando el mandato de CLI [bluemix iam account-user-invite](/docs/cli/reference/bluemix_cli/bx_cli.html#bluemix_iam_account_user_invite), pero debe utilizarse la interfaz de usuario para asignar otro acceso o permisos.

## Acceso de infraestructura

Los permisos reales asignados se limitan automáticamente al subconjunto de permisos que posee. Para obtener más información sobre los permisos y las acciones que puede llevar a cabo el usuario, consulte [Permisos de infraestructura](/docs/iam/users_roles.html#infrapermissions).

1. Desde la pantalla **Invitar usuarios**, expanda la sección **Acceso de infraestructura**.
2. Seleccione un permiso para definir el ámbito del acceso.

Para obtener información sobre la configuración del acceso para los usuarios después de que se añadan a su cuenta, consulte [Gestión de usuarios y acceso](/docs/iam/iamusermanage.html).
