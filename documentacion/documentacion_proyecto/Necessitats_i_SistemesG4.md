
# Estudio de sistemas operativos para nuestra empresa

## 1. Comunicaciones: MikroTik y Ubuntu Server

| Sistema | Ventajas | Inconvenientes | Coste |
|---|---|---|---|
| **MikroTik RouterOS** | Firewall, VLAN, VPN y enrutamiento desde una interfaz centralizada. | Requiere aprender su configuración. | Licencia incluida en los routers compatibles. |
| **pfSense CE** | Cortafuegos, VPN y administración web. | Necesita hardware compatible y mantenimiento propio. | Gratuito. |
| **Ubuntu Server** | Flexible, permite instalar DNS, VPN y otras herramientas. | Muchos servicios requieren configuración manual. | Gratuito; soporte profesional opcional. |

### Eleccion final

Elegimos MikroTik RouterOS para gestionar la red y Ubuntu Server para proporcionar servicios adicionales. Así separamos las funciones de red de los servicios internos.

---

## 2. Virtualización: Proxmox VE

| Sistema | Ventajas | Inconvenientes | Coste |
|---|---|---|---|
| **Proxmox VE** | Máquinas virtuales, contenedores, copias de seguridad y administración web. | Requiere conocimientos de administración de servidores. | Gratuito; suscripción opcional para servicios empresariales. |
| **VMware vSphere** | Solución profesional con herramientas avanzadas de virtualización. | Sus condiciones comerciales y licencias pueden resultar complejas. | Depende de la oferta contratada. |
| **Microsoft Hyper-V** | Integración con Windows Server y tecnologías Microsoft. | Las condiciones y funciones disponibles dependen de la edición y del escenario. | Puede estar incluido en determinadas ediciones de Windows Server. |

### Elección final

Elegimos Proxmox VE para virtualizar y aprovechar mejor los recursos y administrar las máquinas desde una interfaz sencilla. 

---

## 3. Gestión centralizada: Windows Server

| Sistema | Ventajas | Inconvenientes | Coste |
|---|---|---|---|
| **Windows Server con Active Directory** | Dominios, usuarios, grupos, políticas de grupo y permisos centralizados. | Requiere licencias y conocimientos de administración. | De pago; pueden ser necesarias licencias CAL. |
| **Samba AD DC** | Puede proporcionar servicios de dominio compatibles con clientes Windows. | Algunas funciones y compatibilidades difieren de Active Directory de Microsoft. | Gratuito. |
| **FreeIPA** | Gestión centralizada de identidades, políticas y autenticación en entornos Linux. | No sustituye directamente todas las funciones de Active Directory para equipos Windows. | Gratuito. |

### Elección final

Elegimos Windows Server con Active Directory porque tenemos seis equipos Windows y necesitamos gestionar sus cuentas, permisos y configuraciones desde un único lugar. Las políticas de grupo permiten aplicar configuraciones de seguridad sin tener que configurar cada ordenador manualmente.

---

## 4. Clientes: Windows 11 y Linux Mint

| Sistema | Ventajas | Inconvenientes | Coste |
|---|---|---|---|
| **Windows 11 Pro** | Compatible con aplicaciones empresariales, unión a dominios de Active Directory y políticas corporativas. | Requiere una licencia válida si no está incluida en el equipo. | Depende de la licencia o del equipo. |
| **Linux Mint** | Gratuito, relativamente ligero y adecuado para desarrollo y administración. | Algunas aplicaciones empresariales solo están disponibles para Windows. | Gratuito. |
| **Ubuntu Desktop** | Amplio soporte comunitario y buenas herramientas de desarrollo. | Puede requerir alternativas a programas exclusivos de Windows. | Gratuito. |

### Elección final

Utilizaremos Windows 11 Pro en cuatro equipos y Windows con Linux Mint en arranque dual en otros dos.

---

## 5. Datos: TrueNAS

| Sistema | Ventajas | Inconvenientes | Coste |
|---|---|---|---|
| **TrueNAS Community Edition** | Almacenamiento centralizado, ZFS, permisos, instantáneas y compartición de archivos. | Requiere hardware adecuado y conocimientos de almacenamiento. | Gratuito. |
| **OpenMediaVault** | Administración web, carpetas compartidas y extensiones. | Algunas funciones dependen de complementos. | Gratuito. |
| **Windows Server como servidor de archivos** | Integración con Active Directory, permisos NTFS y auditoría. | Consume recursos y requiere licencias adecuadas. | De pago. |

### Elección final

Elegimos TrueNAS Community Edition porque está especializado en almacenamiento y permite compartir archivos mediante SMB, gestionar permisos.

---

## WebGrafia

- [MikroTik RouterOS](https://mikrotik.com/software)
- [pfSense](https://www.pfsense.org/)
- [Ubuntu Server](https://ubuntu.com/server)
- [Proxmox VE](https://www.proxmox.com/en/proxmox-virtual-environment/overview)
- [Microsoft Windows Server](https://www.microsoft.com/windows-server)
- [Samba](https://www.samba.org/)
- [FreeIPA](https://www.freeipa.org/)
- [Windows 11](https://www.microsoft.com/windows/business)
- [Linux Mint](https://linuxmint.com/)
- [Ubuntu Desktop](https://ubuntu.com/desktop)
- [TrueNAS](https://www.truenas.com/)
- [OpenMediaVault](https://www.openmediavault.org/)

