# 🚀 Pull Request: Validación de Calidad Salesforce

## 📘 Documentación de Referencia
Antes de solicitar revisión, asegúrate de haber consultado los estándares vigentes:
- [Manual de Estándares Salesforce 2026](https://wiki.meli.com/salesforce-2026)
- [Guía de Named Credentials](https://wiki.meli.com/named-credentials)

---

## 🛠️ Checklist de Auto-Validación (Obligatorio)
*El desarrollador debe marcar estas casillas antes de asignar revisores.*

### Seguridad y Datos
- [ ] **Contexto DML:** He especificado explícitamente `as user` (o `as system` con justificación).
- [ ] **Consultas SOQL:** Todos los queries utilizan `WITH SECURITY_ENFORCED` o `USER_MODE`.
- [ ] **Named Credentials:** No hay URLs ni Secretos hardcodeados; se usan Callouts a credenciales nombradas.

### Calidad de Código (Clean Code)
- [ ] **Debugs:** Se eliminaron todos los `System.debug()`.
- [ ] **Código Comentado:** No hay bloques de código muerto o comentado.
- [ ] **Naming:** Las variables nuevas siguen la convención `camelCase`.

### Metadata y Otros
- [ ] **Platform Events (__e):** Todos los campos nuevos tienen el tag `<description>` (Origen -> Impacto).
- [ ] **Versión API:** Los componentes nuevos están en versión **60.0** o superior.
- [ ] **Custom Labels:** Todos los mensajes al usuario final usan etiquetas con traducción (ES/PT).

---

## 📝 Descripción de los Cambios
*Explica brevemente qué hace este cambio y por qué es necesario.*

> [Escribe aquí...]

---
**Nota:** Esta es una validación manual obligatoria del desarrollador. Al marcar las casillas, confirmas que el código cumple con la vara de calidad MeLi.
