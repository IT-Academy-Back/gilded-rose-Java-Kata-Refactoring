
![Refactoring Kata](https://img.shields.io/badge/Kata%20Refactoring-Easy-brightgreen?style=flat-square)
![Kata CI Test](https://img.shields.io/github/actions/workflow/status/IT-Academy-Back/java-template-with-analysis/ci.yml?branch=main&label=CI%20Kata%20Test&style=flat-square)
[![Coverage](https://sonarcloud.io/api/project_badges/measure?project=IT-Academy-Back_java-template-with-analysis&metric=coverage)](https://sonarcloud.io/summary/new_code?id=IT-Academy-Back_kata-rpg-refactoring)
[![Quality Gate Status](https://sonarcloud.io/api/project_badges/measure?project=IT-Academy-Back_java-template-with-analysis&metric=alert_status)](https://sonarcloud.io/summary/new_code?id=IT-Academy-Back_java-template-with-analysis)

> ⚠️ **Nota:** Los badges de CI y Cobertura apunta al repositorio original.
> Si haces un *fork* o usas este proyecto como *template*, cambia las URLs de los badges para que apunten a tu propio repositorio.
---

### 📊 **Cobertura de código con JaCoCo**

Este proyecto genera automáticamente un informe de cobertura tras cada *push* a `main`.  
Puedes consultar el reporte accediendo a:
[Cobertura de código](https://IT-Academy-Back.github.io/java-template-with-analysis)

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
