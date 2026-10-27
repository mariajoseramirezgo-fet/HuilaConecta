# HuilaConecta 

Página web interactiva orientada a dinamizar y promover el turismo regional en el departamento del Huila.

---

##  1. Información General del Proyecto

* **Descripción:** HuilaConecta es una plataforma digital de turismo interactivo diseñada para conectar a viajeros, turistas locales y entusiastas de la cultura opita con los principales destinos, experiencias, gastronomía y comunidad del departamento del Huila.
* **Público Objetivo:** Viajeros, turistas, guías locales y ciudadanos interesados en descubrir atractivos icónicos como San Agustín, el Desierto de la Tatacoa y la oferta cultural de la región.
* **Propósito:** Proveer una guía de viaje accesible, moderna y responsiva que permita explorar destinos, gestionar perfiles de usuario e interactuar mediante un muro comunitario dinámico.

---

##  2. Mapa del Sitio y Estructura de Secciones

La pagina web se estructura con navegación fluida mediante un menú inferior (*Bottom Navigation*):

1. **Inicio / Exploración:** Vista principal con destinos destacados y buscador rápido.
2. **Destinos (San Agustín / Tatacoa):** Información detallada de atractivos turísticos con galerías de fotos reales.
3. **Comunidad:** Muro interactivo donde los usuarios pueden publicar experiencias, compartir reseñas y dar 'Me gusta' con persistencia local (`localStorage`).
4. **Mapa / Rutas:** Visualización de puntos clave de interés regional.
5. **Perfil de Usuario:** Gestión de cuenta con validación de seguridad para cambio de contraseña y carga de foto de perfil personalizada.

Se puede encontrar de forma visual en la pagina **fase 3. Flujo de usuario y wireframes** en este enlace de figma: https://www.figma.com/design/3DTIIhV2poGFdg6UPjdPzD/Dise%C3%B1o-de-una-app-m%C3%B3vil-con-Figma-y-Google-Stitch?node-id=12-2&t=zJ8KJDhgOU7cxozx-1

---

##  3. Identidad Visual (Paleta de Colores y Tipografía)

* **Paleta 60-30-10:**
  * **60% (Dominante):** Azul oscuro profundo (`#020618`) para fondos y estructura general en modo oscuro.
  * **30% (Secundario):** Tonos de soporte (`#1E293B` / `#FFFDF9`) en tarjetas y contenedores.
  * **10% (Acento):** Naranja vibrante (`#EA580C`) y Amarillo vivo (`#FACC15`) para llamadas a la acción (*Call to Action*).
* **Tipografía:**
  * **Títulos:** *Outfit* (modernidad y carácter visual).
  * **Cuerpo y Textos:** *Inter* (legibilidad y limpieza en pantallas móviles).
* **Accesibilidad:** Verificado mediante estándares de contraste para garantizar una experiencia óptima y cumplimiento en herramientas de validación.

La paleta **60-30-10** se encuentra en el mismo enlace de figma en la **Fase 2. Fundamentos Visuales**
---

## 📊 4. Bitácora de Prompts de ajustes e Iteraciones

| # Iteración | Prompt de Ajuste Enviado | Problema que Buscaba Resolver | Resultado Obtenido | ¿Funcionó? |
| --- | --- | --- | --- | --- |
| 1 | Sincroniza las clases de Tailwind para que los colores de las letras y textos se adapten correctamente y mantengan una lectura óptima al cambiar entre el modo claro y el modo oscuro. | Corregir problemas de contraste y legibilidad en los textos al alternar dinámicamente entre el modo claro y oscuro. | Se aplicaron las clases de variante dark: de forma coherente en los selectores de texto y contenedores. | Sí |
| 2 | Reemplaza los fondos degradados de todas las tarjetas por imágenes reales del Huila y ajusta su diseño. | Eliminar los recuadros de colores planos o degradados y mostrar fotografías representativas en todas las secciones de la página web. | Se actualizaron los contenedores para cargar imágenes reales con el ajuste responsivo adecuado y buen contraste de los textos. | Sí |
| 3 | Implementa la funcionalidad de cambiar contraseña con validación de formato y permite subir una foto de perfil en la sección de usuario. | Añadir interactividad real de gestión de cuenta en el perfil (validación de seguridad en contraseña y carga de imagen local). | Se programó la lógica de validación de campos y carga de archivos locales para el perfil de usuario. | Sí |
| 4 | Cambia el color de fondo al tono azul oscuro #020618 e incluye fotos reales en todas las secciones de la interfaz. | Ajustar el color de fondo general al tono azul profundo solicitado y garantizar soporte multimedia visual en cada vista. | Se aplicó el color de fondo #020618 y se aseguraron las imágenes en todas las tarjetas de la SPA. | Sí |
| 5 | Haz que las nuevas publicaciones de la comunidad se vayan acumulando y agregando a la pantalla sin borrar las anteriores, y que al dar 'Me gusta' el botón cambie a color rojo para que el cambio sea evidente. | Evitar que una nueva publicación reemplace a las existentes en el muro comunitario y dar retroalimentación visual clara (botón rojo) al interactuar con el 'Me gusta'. | Se ajustó la lógica de acumulación en arrays de JavaScript y la actualización visual dinámica del botón de interacción. | Sí |

---
