# PROTOCOLO-DE-SEGURIDAD-PARA-EL-TRABAJO-REMOTO
El acceso a las plataformas de la empresa debe estar protegido por múltiples capas de seguridad para prevenir el robo de credenciales.
**Versión:** 1.0

**Departamento:** Seguridad de la Información / IT

**Alcance:** Todo el personal con acceso a redes y datos corporativos.
## 1. Gestión de Identidad y Acceso Seguro

El acceso a las plataformas de la empresa debe estar protegido por múltiples capas de seguridad para prevenir el robo de credenciales.

### 🔑 Políticas de Contraseñas

-   **Longitud mínima:** 14 caracteres.
    
-   **Formato:** Uso obligatorio de frases de seguridad (_passphrases_) que incluyan mayúsculas, números y símbolos.
    
-   **Prohibición:** No se permite la reutilización de contraseñas personales para cuentas corporativas.
    

### 🔐 Autenticación de Doble Factor (MFA)

Es obligatorio el uso de un segundo factor de autenticación para todos los servicios (Correo, Slack, VPN).

-   **Método preferido:** Aplicaciones de autenticación (Google Authenticator, Microsoft Authenticator).
    
-   **Método crítico:** Llaves de seguridad físicas (Yubikey) para personal con acceso a datos sensibles.
    

----------

## 2. Seguridad en la Conexión y Redes

El personal remoto debe garantizar que el canal de comunicación entre su hogar y la empresa sea privado.

### 🌐 Uso de VPN (Virtual Private Network)

-   Todo acceso a servidores internos o herramientas de gestión debe realizarse exclusivamente a través de la **VPN corporativa**.
    
-   Queda estrictamente prohibido el uso de redes Wi-Fi públicas (cafeterías, aeropuertos) sin el túnel VPN activo.
    

### 📡 Seguridad del Router Hogareño

-   El router debe tener el firmware actualizado.
    
-   La contraseña del Wi-Fi debe ser robusta y el protocolo de seguridad debe estar configurado en **WPA3** o, en su defecto, **WPA2-AES**.
    

----------

## 3. Protección de Dispositivos y Datos

Los equipos de trabajo son propiedad de la empresa y deben ser tratados como tales.

### 💻 Endpoints (Laptops/Móviles)

-   **Cifrado de disco:** El disco duro debe estar cifrado (BitLocker en Windows o FileVault en macOS).
    
-   **Bloqueo automático:** Configurado a un máximo de 5 minutos de inactividad.
    
-   **Software:** Prohibida la instalación de software no autorizado por el departamento de IT.
    

### 📧 Prevención de Phishing y Malware

-   Verificación obligatoria de la dirección del remitente antes de hacer clic en cualquier enlace.
    
-   Reporte inmediato de correos sospechosos al canal de Slack `#it-security`.
    

----------

## ❓ FAQ para Empleados

**¿Puedo prestarle mi computadora de trabajo a un familiar?** No. El equipo es de uso exclusivo para tareas laborales y contiene información confidencial protegida por acuerdos de privacidad.

**¿Qué hago si pierdo mi equipo o sospecho que fui hackeado?** Debes reportarlo en menos de **30 minutos** al centro de soporte para bloquear los accesos de forma remota.

----------

### 🚀 ¿Cómo usar esto para tu carrera?

1.  **Súbelo a GitHub:** Crea un nuevo repositorio llamado `Ciberseguridad-Corporativa` y guarda este código como `README.md`.
    
2.  **El valor técnico:** En tu entrevista puedes decir: _"Entiendo que el factor humano es el mayor riesgo en seguridad, por eso diseñé protocolos de higiene digital para equipos remotos"_.
    
3.  **Diferenciación:** Mientras otros suben "Hola Mundo", tú estás subiendo **Políticas de Seguridad**.
    
## 📊 Matriz de Clasificación de Riesgos y Respuesta

Para que el personal sepa cómo actuar, utilizamos la siguiente escala de criticidad ante incidentes:

| Nivel de Riesgo | Tipo de Incidente | Acción Inmediata |
| :--- | :--- | :--- |
| 🔴 **Crítico** | Pérdida de equipo o sospecha de acceso externo. | Reporte inmediato (menos de 30 min) y bloqueo de cuentas. |
| 🟡 **Medio** | Recepción de correo sospechoso o Phishing. | Reportar al canal `#it-security` sin hacer clic en enlaces. |
| 🟢 **Bajo** | Fallos en la VPN o actualización de software. | Abrir ticket de soporte estándar. |

### 🛠️ Configuración de Seguridad en el Router
Si trabajas desde casa, tu conexión debe cumplir con estos requisitos mínimos:

| Componente | Configuración Requerida |
| :--- | :--- |
| **Protocolo Wi-Fi** | WPA2-AES o WPA3 |
| **Contraseña Administrativa** | Cambiada (no usar la que viene de fábrica) |
| **SSID** | Nombre genérico (no usar nombres personales) |

---

## 📚 Referencias y Estándares
Este protocolo se basa en los mejores marcos de trabajo de ciberseguridad a nivel mundial:

* **NIST SP 800-46:** Guía para la seguridad del teletrabajo y el acceso remoto. [Ver fuente](https://csrc.nist.gov/publications/detail/sp/800-46/rev-2/final)
* **ISO/IEC 27001:** Estándar internacional para la seguridad de la información.
* **OWASP:** Mejores prácticas para la protección de identidad y contraseñas. [Ver fuente](https://cheatsheetseries.owasp.org/cheatsheets/Authentication_Cheat_Sheet.html)

---

## ❓ Preguntas Frecuentes adicionales

**¿Por qué es obligatorio el uso de la VPN incluso para revisar mi correo?**
La VPN cifra el tráfico de extremo a extremo. Sin ella, en ciertas configuraciones de red, un atacante podría interceptar los datos que viajan entre tu computadora y el servidor de la empresa.

**¿Puedo usar mi computadora personal para trabajar si la mía falla?**
Solo bajo autorización explícita de IT y tras una auditoría rápida del equipo. El uso de equipos personales (BYOD) aumenta el riesgo de fuga de datos si el equipo está infectado con malware previo.
