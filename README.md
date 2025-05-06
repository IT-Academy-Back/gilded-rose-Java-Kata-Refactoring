
![Refactoring Kata](https://img.shields.io/badge/Kata%20Refactoring-Easy-brightgreen?style=flat-square)
![Kata CI Test](https://img.shields.io/github/actions/workflow/status/IT-Academy-Back/gilded-rose-Java-Kata-Refactoring/ci.yml?branch=main&label=CI%20Kata%20Test&style=flat-square)
[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=IT-Academy-Back_gilded-rose-Java-Kata-Refactoring&metric=coverage)](https://sonarcloud.io/summary/new_code?id=IT-Academy-Back_gilded-rose-Java-Kata-Refactoring)
[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=IT-Academy-Back_gilded-rose-Java-Kata-Refactoring&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=IT-Academy-Back_gilded-rose-Java-Kata-Refactoring)

> ⚠️ **Nota:** Los badges de CI y Cobertura apunta al repositorio original.
> Si haces un *fork* o usas este proyecto como *template*, cambia las URLs de los badges para que apunten a tu propio repositorio.
---
# The Gilded Rose Kata

## Enunciado

Bienvenido a la **Kata de Gilded Rose**. Esta kata está diseñada para ayudarte a practicar y mejorar tus habilidades de refactorización en un código heredado.

### Descripción del Problema

Gilded Rose es una pequeña tienda de objetos mágicos, y su sistema de gestión de inventario necesita ser mejorado. Actualmente, el sistema tiene una clase llamada `Item` y una clase `GildedRose` que gestiona el inventario. El código de `GildedRose` es difícil de mantener y debe ser refactorizado sin cambiar su comportamiento.

### Reglas del Inventario

Cada artículo en el inventario tiene las siguientes propiedades:
- `name`: el nombre del artículo.
- `sellIn`: el número de días que quedan para vender el artículo.
- `quality`: un valor que representa lo valioso que es el artículo.

El sistema debe actualizar estas propiedades diariamente de acuerdo con las siguientes reglas:

1. Al final de cada día, el sistema reduce los valores de `sellIn` y `quality` para cada artículo.
2. Una vez que la fecha de venta ha pasado (`sellIn` < 0), la `quality` del artículo disminuye dos veces más rápido.
3. La `quality` de un artículo nunca es negativa.
4. "Aged Brie" incrementa su `quality` a medida que envejece.
5. La `quality` de un artículo nunca es mayor que 50.
6. "Sulfuras", siendo un artículo legendario, nunca tiene que ser vendido ni disminuye su `quality`.
7. "Backstage passes", como los de un concierto de TAFKAL80ETC, incrementan su `quality` a medida que su `sellIn` se aproxima:
    - `quality` incrementa en 2 cuando faltan 10 días o menos.
    - `quality` incrementa en 3 cuando faltan 5 días o menos.
    - `quality` cae a 0 después del concierto.
9. "Conjured" es un **nuevo tipo de artículo** que se degrada el doble de rápido que los artículos normales.

### Requisitos

- Tu tarea 1: es refactorizar el código de `GildedRose` sin cambiar el comportamiento existente. Debes hacer que el código sea más limpio, mantenible y preparado para futuras extensiones.
- Tu tarea 2: es añadir un nuevo tipo de artículo llamado "Conjured". Debe seguir las reglas de degradación de calidad de los artículos "Conjured".
- Por supuesto debes añadir los tests necesarios para comprobar que el código sigue funcionando correctamente después de la refactorización y la adición del nuevo tipo de artículo.
- Asegúrate de que el código sigue funcionando correctamente después de la refactorización. Puedes usar los tests existentes para comprobarlo.
- Puedes añadir tests adicionales si lo consideras necesario.

### Notas

- No puedes cambiar la clase `Item` ni su propiedad `name`.
- El método `updateQuality` debe permanecer en la clase `GildedRose`.
- No puedes cambiar la firma del método `updateQuality`.
- Puedes hacer cualquier cambio en la clase `GildedRose` siempre y cuando no cambie su comportamiento.

---

### 📊 **Cobertura de código con JaCoCo**

Este proyecto genera automáticamente un informe de cobertura tras cada *push* a `main`.  
Puedes consultar el reporte accediendo a:
[Cobertura de código](https://IT-Academy-Back.github.io/gilded-rose-Java-Kata-Refactoring)

```
https://TU_USUARIO.github.io/TU_REPOSITORIO/
```

> 📝 Si usas este repositorio como template, **recuerda cambiar la URL anterior** reemplazando `TU_USUARIO` y `TU_REPOSITORIO` por los tuyos.

> 📄 GitHub Pages se activará automáticamente tras el primer push a `main`, cuando se genere la rama `gh-pages`.

> ⚠️ Si has hecho un **fork** o un **clone**, ve a `Settings → Pages` y selecciona la rama `gh-pages`, carpeta `/ (root)` para activar GitHub Pages manualmente.


## 📈 Análisis de calidad con SonarCloud

Este proyecto también está conectado con [SonarCloud](https://sonarcloud.io), que analiza automáticamente la calidad del código en cada push.

🔍 SonarCloud evalúa:

- Errores y bugs potenciales
- Vulnerabilidades de seguridad
- Código duplicado
- Calidad del código y mantenibilidad
- Cobertura de tests (a partir de JaCoCo)

🔗 Puedes consultar el análisis de este proyecto en:

👉 [Ver análisis en SonarCloud](https://sonarcloud.io/project/overview?id=IT-Academy-Back_java-template-with-analysis)

🛠️ Si usas este repositorio como template:
1. Crea tu propia organización en SonarCloud.
2. Vincula tu nuevo repositorio.
3. Actualiza las variables `sonar.projectKey` y `sonar.organization` en el workflow de GitHub Actions.
4. **Crea un token en SonarCloud y guárdalo como `SONAR_TOKEN` en los Secrets de tu repositorio en GitHub.**

⚠️ Desactiva el análisis automático en la configuración de SonarCloud si estás ejecutando el análisis desde GitHub Actions (para evitar errores por duplicación de análisis).

📛 También puedes añadir este badge al README para mostrar la cobertura directamente desde SonarCloud:

```markdown
[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=TU-USUARIO-GITHUB_TU-REPOSITORIO&metric=coverage)](https://sonarcloud.io/summary/new_code?id=TU-USUARIO-GITHUB_TU-REPOSITORIO)
```
---
