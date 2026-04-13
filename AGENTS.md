# AGENTS.md — awesome-cantabria

## Propósito

Selección de software open source que da **soporte específico a Cantabria** — su gobierno autonómico, ayuntamientos, universidades, empresas, infraestructuras y patrimonio. Todo el contenido en español. El foco es Cantabria: el software debe dirigirse específicamente a esta comunidad autónoma o a sus municipios.

## Ámbito

- **1 provincia** (Cantabria es comunidad autónoma uniprovincial), con **102 municipios**.
- Principales ciudades: Santander (capital), Torrelavega, Castro Urdiales, Camargo, Piélagos, El Astillero, Laredo, Santoña, Reinosa.
- **Universidades**: UC (Universidad de Cantabria), UNEATLANTICO (Universidad Europea del Atlántico).
- **Instituciones**: Gobierno de Cantabria, ICANE (Instituto Cántabro de Estadística), CANTUR (Sociedad Regional Cántabra de Promoción Turística), SCS (Servicio Cántabro de Salud), TUS (Transportes Urbanos de Santander).

## Criterios de inclusión

### Incluir

- Software que interactúa con el **Gobierno de Cantabria** o sus organismos (Sede Electrónica, Portal de Transparencia, datos abiertos).
- Herramientas para **ayuntamientos** de Cantabria.
- Software de **universidades cántabras** (UC, UNEATLANTICO) cuando sea específico de la región o la universidad.
- Herramientas de **datos abiertos** de Cantabria (ICANE, datos.cantabria.es).
- Software del proyecto **SmartSantander** (plataforma IoT de referencia mundial).
- Herramientas de **transporte** cántabro (TUS, FEVE, cercanías, puertos).
- Herramientas de **cartografía y SIG** específicas de Cantabria.
- Software sobre **playas y costa** cántabra.
- Herramientas de **turismo y patrimonio** de la región (CANTUR, Altamira, Picos de Europa).
- Software de **meteorología** regional.
- Proyectos del **sistema sanitario cántabro** (SCS, Hospital Valdecilla).
- Software **educativo** específico de la región.
- Proyectos de **smart cities** para ciudades cántabras.
- Software sobre **medio ambiente** regional (Parque Natural de Cabárceno, Picos de Europa, bahía de Santander).

### No incluir

- Software **genérico** que funciona en toda España sin funcionalidad específica de Cantabria — eso pertenece a awesome-spain.
- Software de **ámbito europeo** — eso pertenece a awesome-europe.
- Software de **otras comunidades autónomas** españolas.
- Software creado por cántabros que **no tiene funcionalidad específica** de la región.
- Repositorios **archivados o de solo lectura** — van a `DELETED.md`.
- Repos donde el autor indica que el proyecto está **roto, sin mantenimiento o deprecado**.
- Repos **sin README significativo** o que son claramente repos de test/experimento.
- Ejercicios de clase o trabajos académicos sin utilidad real.

### Zona gris — usar criterio

- Proyectos de universidades cántabras que podrían ser genéricos — incluir si tienen datos o configuración específica de Cantabria.
- Software que cubre Cantabria junto con otras regiones — incluir si Cantabria es un foco principal.

## Estándares de calidad

**Mismo listón que [awesome-spain](https://github.com/GeiserX/awesome-spain):**

- **No repos archivados**: si se descubre archivado tras la inclusión, mover a `DELETED.md` inmediatamente.
- **No repos extremadamente sin mantenimiento**: al menos un commit en los últimos 3 años, salvo que sea un proyecto claramente estable/completo.
- **No repos rotos**: si el README dice «deprecated», «no longer maintained», «use X instead» o similar — no incluir. Mover a `DELETED.md` si ya está listado.
- **Estrellas mínimas**: preferir repos con al menos unas pocas estrellas, pero herramientas nicho excepcionales con 0-1 estrellas pueden incluirse si cubren un hueco importante.
- **Verificar cada repo** antes de añadir: comprobar `archived`, `pushed_at`, `stargazers_count` vía `gh api repos/owner/name`.

## Formato de entrada

```markdown
- [Nombre](https://github.com/owner/repo) [![Stars](...)](stargazers) [![Last Commit](...)](commits) [![Language](...)](repo) [![License](...)](LICENSE) [![Tag](...)](url) - Descripción que empieza en mayúscula y termina con punto.
```

Las insignias se generan automáticamente con `scripts/transform-readme.py`. Para contribuir, basta con añadir la entrada en formato simple:

```markdown
- [Nombre](https://github.com/owner/repo) - Descripción que empieza en mayúscula y termina con punto.
```

- La descripción **no debe empezar con el nombre** del proyecto.
- Máximo una línea por entrada.
- Validar con awesome-lint-extra: `python3 lint.py` o mediante el workflow de CI.
- Entradas en **orden alfabético** dentro de cada categoría.
- Categorías en **orden alfabético** en el índice y en el cuerpo del documento.
- Entradas en `DELETED.md` también en **orden alfabético** dentro de cada sección.

## Verificación antes de añadir

Antes de incluir un repositorio, comprobar:

- **Existe y es público**: el enlace de GitHub funciona y el repo no es privado.
- **No está archivado o de solo lectura**: si archivado, va a `DELETED.md` (sección «Archivados»).
- **No está deprecado**: comprobar si el README dice «deprecated», «unmaintained», «broken», «use X instead».
- **Actividad razonable**: al menos un commit en los últimos 3 años, salvo que sea un proyecto estable/completo.
- **No es un duplicado**: cruzar con `README.md` y `DELETED.md`.
- **Calidad mínima**: tiene documentación (README) y no es un repositorio vacío o de test.

## Pull requests y contribuciones

- Las PRs deben usar la plantilla en `.github/PULL_REQUEST_TEMPLATE.md`.
- **Obligatorio**: incluir en la PR la **URL del servicio, API o institución cántabra** a la que el software da soporte.
- Plantillas de issues disponibles para sugerir proyectos (`anadir-proyecto.md`) y solicitar retirada (`retirar-proyecto.md`).

## Estructura

- Secciones con `##`, subsecciones con `###`.
- Índice de contenido al principio entre comentarios `<!--lint disable/enable awesome-list-item-->`.
- Al final: sección Contribuir, Nota y Descargo de responsabilidad (como párrafos en negrita, no encabezados ##).

## Temas prohibidos

No se aceptan proyectos relacionados con: pornografía, contenido NSFW, loterías o apuestas, religión, política partidista.

## Difusión

- Notificar a los propietarios de repos abriendo un issue titulado «Listado en awesome-cantabria» con un breve mensaje en español (tuteo) ofreciendo retirar si lo prefieren. Solo 1 issue por organización/usuario — no spamear repos del mismo propietario.
- Publicar en comunidades cántabras (Reddit, foros de la UC, Telegram de devs cántabros, Coders Cantabria) tras alcanzar masa crítica.
- Enviar PR a [sindresorhus/awesome](https://github.com/sindresorhus/awesome) tras 30 días desde la creación del repo.

## Aprendizajes

- ICANE (Instituto Cántabro de Estadística) tiene organización GitHub `icane` con repos útiles: pyaxis (20 estrellas, activo), etlstat, economic-indicators, demographic-indicators, ods-cantabria, ckanext-federgob, icane-metadata.
- `predicador37` es un desarrollador del ICANE con repos adicionales: pyicane (wrapper API ICANE), icanechecker.
- El proyecto **SmartSantander** es una iniciativa IoT de referencia mundial con sensores por toda la ciudad. Repos en `Predictia/smartsantander` y `Predictia/smartmap`.
- **Coders Cantabria** (`coders-cantabria`) es una comunidad de desarrolladores cántabros, pero sus repos son charlas y workshops genéricos — no específicos de Cantabria.
- La búsqueda de «Santander» produce muchos falsos positivos por el banco Santander y por Santander (Colombia).
- La Universidad de Cantabria no tiene organización GitHub oficial. Los repos son de profesores/estudiantes individuales.
- `casadoj/Clases` (19 estrellas) es material del Master en Gestión Integral de Sistemas Hídricos de la UC — incluible por su contenido académico de calidad.
- `fuentesp/fogsim` (4 estrellas) es un simulador de redes del Departamento de Informática de la UC.
- `steven2358/Cantabria-beamer-template` (3 estrellas) es una plantilla Beamer para la UC.
- `oscaruiz/playas-cantabria` (2 estrellas, activo 2026) es un visor de estado de playas cántabras.
- `masterdatascience-UIMP-UC` es la organización del Master en Data Science UIMP-UC con repo icane-panorama.
- Muchos repos con «cantabria» en GitHub son ejercicios de clase o sitios web personales sin utilidad técnica.

*Generated by [LynxPrompt](https://lynxprompt.com) CLI*
