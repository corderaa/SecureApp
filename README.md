# SecureApp – Aplicación Web con Modo Vulnerable y Seguro

**SecureNotes** es una aplicación web desarrollada con Spring Boot que simula un entorno inseguro y seguro para demostrar cómo aplicar buenas prácticas de ciberseguridad en el desarrollo de software.

Este proyecto es ideal para desarrolladores interesados en aprender sobre las vulnerabilidades más comunes (OWASP Top 10) y cómo prevenirlas con Spring Security.

---

## Características del Proyecto

- **CRUD de notas privadas**
- **Registro e inicio de sesión de usuarios**
- **Modo "Vulnerable" vs. "Seguro"** (seleccionable desde configuración)
- **Aplicación de Spring Security en la versión segura**
- **Demostraciones de ataques comunes:**
  - Inyección SQL
  - Cross-Site Scripting (XSS)
  - CSRF (Cross-Site Request Forgery)
  - Fugas de sesión

---

## Tecnologías utilizadas

- Java 17+
- Spring Boot
- Spring Security
- Spring Data JPA
- H2 (modo demo) o PostgreSQL
- Thymeleaf
- Bootstrap (UI básica)

---

## Estructura del Proyecto
```
secure-notes/
├── src/
│ ├── main/
│ │ ├── java/com/example/securenotes/
│ │ │ ├── config/ # Seguridad y configuración de modos
│ │ │ ├── controller/ # Controladores web
│ │ │ ├── model/ # Entidades
│ │ │ ├── repository/ # Repositorios JPA
│ │ │ └── service/ # Lógica de negocio
│ ├── resources/
│ │ ├── templates/ # Vistas Thymeleaf
│ │ └── application.yml # Configuración del modo seguro/vulnerable
```

## Cómo usar

### 1. Clonar el repositorio

```bash
git clone https://github.com/tuusuario/secure-notes.git
cd secure-notes
./mvnw spring-boot:run
