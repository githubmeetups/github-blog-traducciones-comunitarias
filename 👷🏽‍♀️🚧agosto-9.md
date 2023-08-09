guía para preparar su repositorio para la colaboración- TRADUCCION NO FINAL

https://github.blog/2023-08-04-a-checklist-and-guide-to-get-your-repository-collaboration-ready/

A Checklist & Guide to get your Repository Collaboration-Ready

**Guía para Preparar tu Repositorio para la Colaboración**

Una Lista de Verificación y Guía para Preparar tu Repositorio para la Colaboración

¿Eres nuevo en GitHub o llevas un tiempo usándolo? Si quieres ir al grano, ve al final para obtener una lista de verificación imprimible que puedes usar para asegurarte de que has cubierto todos los aspectos necesarios para hacer que tu repositorio esté listo para la colaboración.

Mi hija tiene un par de jerbos como mascotas. Son geniales, pero no son las criaturas más complejas de cuidar. Necesitan que limpien su jaula de vez en cuando, que les rellenen su comida y agua, y puede que necesiten que un vecino los cuide si nos ausentamos por un tiempo. Pero algún día, podría tener una mascota que requiera más cuidados y atención, como un gato o un perro, que necesitará ser jugado y cuidado todos los días. Por lo tanto, querrá tener algunos buenos amigos que conozcan a su mascota y puedan ser sus compañeros cuando esté ausente. Y algún día, incluso podría tener un hijo propio, lo que hará que sus conexiones con la comunidad y la familia sean aún más importantes. Como dice el refrán, se necesita una aldea para criar a un niño.

Lo mismo ocurre con los proyectos de código. Mis colegas y yo a menudo nos referimos a nuestros proyectos como "mascotas" o incluso "niños" (a veces en tono de broma, a veces con obsesión). Dedicamos mucha de nuestra propia atención y cuidado a ellos, pero puede ser fácil olvidar lo importantes que pueden ser las contribuciones de la comunidad para su éxito. En el mundo del desarrollo de software, la colaboración puede marcar la diferencia entre un lanzamiento frágil de último minuto y un proyecto confiable, mantenible y sin problemas. Ya sea que hayas estado programando durante un día o una década, tus colegas están ahí para ayudarte a fortalecer tu trabajo. Pero solo pueden ayudar si les has proporcionado las herramientas necesarias para hacerlo.

Tu responsabilidad principal como creador o mantenedor de un repositorio es asegurarte de que otros puedan usar, entender e incluso contribuir adecuadamente al proyecto. GitHub está aquí para apoyar esa misión, pero asegurarse de que un repositorio esté listo para la colaboración requiere un poco más de esfuerzo que simplemente usar "git clone". Así que sigue leyendo para aprender acerca de las configuraciones, el contenido y los comportamientos que te ayudarán a tener éxito.

1. Configuraciones del Repositorio

Las configuraciones de tu repositorio establecen la base para la colaboración. Determinan quiénes pueden ver y contribuir a tu proyecto, cómo se revisan las contribuciones y qué sucede con esas contribuciones una vez que se envían. Utilizadas correctamente, pueden fomentar un entorno en el que los colaboradores de todo el mundo encuentren, utilicen y ayuden a construir tu proyecto. En un entorno corporativo, ayudan a cambiar a los desarrolladores de un modo de pensamiento/construcción aislado a una mentalidad de "buscar primero, colaborar primero". Esta práctica, conocida como "innersourcing", reduce el trabajo redundante y acelera toda la empresa.

Visibilidad
Tu objetivo es maximizar las contribuciones y el reuso, pero esto no siempre significa hacer público tu repositorio, especialmente en un entorno corporativo donde la privacidad de la información es importante. Tienes varias opciones disponibles en la pestaña "Configuración" de tu repositorio:

- **Público:** permite que cualquier persona en el mundo vea y copie tu código, y generalmente les permite crear problemas o solicitudes de extracción, para que puedan proporcionar comentarios sobre si funciona bien o incluso sugerir (pero no obligar) cambios para mejorarlo. Esto es genial en general para proyectos personales que no contienen información protegida (¿todas esas claves están almacenadas por separado, ¿verdad?), pero solo para ciertos proyectos "bendecidos" de la empresa.

- **Interno:** es un nivel de visibilidad especial utilizado por GitHub Enterprise, que permite a cualquier persona dentro de tu organización ver el repositorio, pero nadie fuera del mundo exterior. Generalmente sugerimos esto como el nivel predeterminado para proyectos corporativos que no tienen información sensible aislada (por ejemplo, datos específicos del cliente o lógica que solo un grupo específico debería conocer).

- **Privado:** es la opción más restrictiva y puede ser perjudicial para la colaboración. Usa esta opción con moderación y, si lo haces, asegúrate de invitar a algunos...
  
- **Colaboradores:** son individuos o equipos específicos a los que invitas a formar parte de tu proyecto. Se les pueden asignar roles específicos como "Lectura" (que les permite ver tu repositorio privado), "Escritura" (que les permite comprometerse directamente o gestionar Solicitudes de extracción), "Administrador" y muchos otros.

Protege la rama principal
Si bien deseas maximizar la cantidad de personas que pueden ver y contribuir a tu proyecto, aún necesitas asegurarte de que sus contribuciones sean revisadas adecuadamente, tanto por los miembros de tu equipo central como por la automatización. En la mayoría de los casos, querrás crear una regla de repositorio (el reemplazo moderno para la protección de ramas) en tu rama principal y configurarla para requerir una solicitud de extracción antes de permitir la fusión. Al exigir al menos un aprobador, idealmente uno de tu archivo CODEOWNERS (discutido en la siguiente sección), garantizarás que otro ser humano revise cada conjunto de cambios. Además, querrás que se ejecuten herramientas automatizadas como pruebas unitarias en cada solicitud de extracción; estas se conocen como comprobaciones de estado y se tratarán en la sección de "automatización/comprobaciones" a continuación.

2. Contenido del Repositorio

Los proyectos de software no solo consisten en código. Tu repositorio debe actuar como una guía para los colaboradores, permitiéndoles saber por qué existe, cómo usarlo adecuadamente y las mejores formas de contribuir. Agregar algunos archivos clave (generalmente escritos en formato markdown) ayudará a otras personas a descubrir tu proyecto y comprender cómo colaborar de manera efectiva:

- **README.md:** Este es el primer archivo que los visitantes de tu repositorio verán, por lo que es fundamental incluirlo en tu repositorio. Debería describir qué hace tu proyecto, cómo usar el repositorio y cualquier configuración necesaria. Además, un buen README incluye la misión del proyecto, lo que

 pretende hacer y por qué existe. Por último, asegúrate de describir cómo y por quién se mantiene el proyecto.

- **LICENSE.md:** Un archivo de licencia define lo que otros pueden y no pueden hacer con tu código y otro contenido. Ya sea que tu objetivo sea permitir el uso sin restricciones de tu proyecto o agregar restricciones especiales a su uso y distribución, es crucial incluir una licencia. Visita choosealicense.com para obtener orientación sobre qué licencia podría ser la mejor para tu proyecto, luego agrégala a tu repositorio.

- **CONTRIBUTING.md:** Puedes reducir la confusión y la fricción que los posibles contribuyentes (y tú) enfrentan definiendo claramente por qué y cómo otros pueden contribuir con nuevo código, documentación, arte u otros elementos a tu proyecto. Si los pasos de contribución son muy simples, podrías incluirlos en tu archivo README; pero si encuentras que se requiere más de un párrafo o dos (y generalmente lo es), es mejor crear un archivo separado. Debería incluir información sobre los tipos de contribuciones que estás buscando, cómo proponer una nueva función o corrección de errores, el proceso para enviar solicitudes de extracción y cualquier estándar de codificación específico o pautas de estilo que los colaboradores deban seguir. Para un buen ejemplo, echa un vistazo a la guía del colaborador del proyecto de documentación de GitHub.

- **CODEOWNERS:** Un archivo CODEOWNERS asigna uno o más usuarios que serán responsables del código en una parte específica de tu repositorio. Según lo especificado en la configuración del repositorio, estas personas serán solicitadas automáticamente para revisión cuando alguien abra una solicitud de extracción que modifique el código que poseen. A diferencia de los otros archivos mencionados aquí, este archivo no debe tener la extensión ".md".

- **CODE_OF_CONDUCT.md:** Un código de conducta establece las normas sociales, las reglas y las responsabilidades que los participantes en tu proyecto deben seguir. Promueve un entorno amigable y respetuoso para la colaboración y es fácil de agregar manualmente o usando una de las plantillas de GitHub.

Con estos archivos en su lugar, tu repositorio será mucho más accesible y comprensible, y deberías comenzar a ver que las contribuciones fluyen con más libertad. Pero si deseas ir aún más lejos, hay más cosas que puedes hacer para preparar tu proyecto para contribuciones saludables.

3. Automatización y Comprobaciones

Es hora de entrar en la Matriz. Como le gusta decir al Agente Smith, "Nunca envíes a un humano a hacer el trabajo de una máquina". Si bien generalmente deseas al menos un revisor humano para cada cambio importante, debes facilitar su trabajo tanto como sea posible. La automatización incorporada de GitHub y el sistema de CI/CD, GitHub Actions, te permiten ejecutar flujos de trabajo en respuesta a cambios en archivos, solicitudes de extracción, disparadores externos como herramientas de chat e incluso como trabajos programados. Veamos algunas formas en que esto puede facilitar la vida de los colaboradores:

- **Linting:** Los linters son herramientas que analizan el código para detectar varios tipos de errores y aplicar un estilo de codificación consistente. Incorporar linters en tu proceso de desarrollo puede mejorar en gran medida la legibilidad y calidad de tu código, lo que facilita a otros comprender y contribuir a tu proyecto. Uno de los más populares es el super linter, que se puede configurar inicialmente en un solo paso de copiar y pegar.

- **Compilación y Pruebas:** Si bien los compiladores y conjuntos de pruebas exactos que ejecutas serán específicos del lenguaje y marco de tu aplicación, la mayoría se pueden ejecutar automáticamente en tu repositorio. Para encontrar los adecuados, busca en la lista de Aplicaciones y Acciones de Construcción y Prueba del Marketplace de GitHub y sigue las instrucciones específicas de tu herramienta preferida. O ejecútalos mediante scripts de línea de comandos y argumentos en tu flujo de trabajo de GitHub Actions.

- **Comprobaciones:** Cuando la información se muestra a los revisores directamente dentro de la solicitud de extracción, facilita su trabajo y elimina la necesidad de que ejecuten manualmente conjuntos de pruebas o recorran una lista de verificación física. Si las comprobaciones automatizadas fallan, incluso podemos bloquear las implementaciones antes de que salgan. Una vez que hayas agregado un linter o un conjunto de pruebas según se describe arriba y se haya ejecutado al menos una vez, considera configurarlo como una comprobación de estado en la configuración de tu repositorio. Esto ayudará a asegurar que tu aplicación se pruebe adecuadamente cada vez que se cree una solicitud de extracción.

Esta no es una lista completa, pero cada proyecto es diferente, así que también considera qué otra calidad de código, gestión de dependencias o automatización previa al lanzamiento podrías querer incluir. Luego, considera cómo deseas implementar el proyecto. En la mayoría de los casos, encontrarás un componente en el Marketplace de GitHub que proporciona una integración llave en mano con tu proveedor de infraestructura favorito, pero también es posible escribir tu propia Acción de GitHub para implementar tu aplicación después de que hayan pasado todas las comprobaciones. Y, para proyectos empresariales de alto volumen, considera el uso de colas de fusión si comienzas a tener problemas de congestión en las ramas que cambian rápidamente.

Con estas herramientas de automatización y comprobaciones en su lugar, puedes tener más confianza en la calidad y consistencia de las contribuciones a tu repositorio y pasar menos tiempo gestionando manualmente el proceso.

4. Seguridad

La seguridad es una preocupación fundamental en cualquier proyecto de software y es especialmente importante cuando se incluyen una variedad de colaboradores que pueden tener diferentes niveles de capacitación en seguridad (o ninguno en absoluto). Afortunadamente, hay algunos pasos simples que puedes tomar para proteger tu código, datos y usuarios de posibles amenazas.

- **Roles:** Decide cuidadosamente qué roles y, por lo tanto, qué permisos le das a los colaboradores en tu repositorio. En general, querrás asignar el rol de "Lectura" al público en general. "Triage" y "Escritura" son para personas de confianza, como miembros de tu empresa o grupo de trabajo (pero solo una vez que se hayan configurado las ramas protegidas y las comprobaciones). Los roles de "Mantenimiento" y "Administrador" son los mejores para tus mantenedores principales, que son responsables de revisar y administrar lo que se implementa.

 También considera que los roles de "Triage" y superiores tienen la capacidad de gestionar problemas, discusiones y comentarios, por lo que querrás confiar en que tienen el compromiso y la experiencia para gestionar el flujo de metadatos en torno a tu proyecto. Los clientes empresariales pueden aprovechar los roles personalizados de repositorio para un control de permisos más granular.

- **Gestión de Secretos:** Los secretos son datos sensibles como claves de API, contraseñas y certificados que necesitas mantener en privado. No quieres que estos se incrusten directamente en tu código o tus registros; en su lugar, debes usar un almacén de claves de terceros o las herramientas nativas de administración de secretos de GitHub, que se encuentran en la sección "Secretos y Variables" de la configuración de tu repositorio. Allí, encontrarás secciones separadas para GitHub Codespaces (una herramienta descrita en la sección "Opciones Avanzadas" a continuación) y para GitHub Actions, ya que es posible que desees usar diferentes secretos durante el desarrollo que durante la producción.

- **Escáneres de Seguridad:** Escanear el código en busca de vulnerabilidades es un tema complejo, pero se divide en tres categorías principales:
  - **Dependencias:** El 80-90% del código de la mayoría de las aplicaciones proviene de fuentes de terceros, los marcos y paquetes en los que construimos el resto de nuestro código. GitHub Dependabot está disponible en todos los repositorios públicos y se puede habilitar automáticamente en toda la organización. Puede alertarte (y ayudarte a proporcionar una solución) siempre que se encuentre una dependencia insegura. Para asegurarte de que Dependabot esté en funcionamiento, verifica la pestaña "seguridad" en la parte superior de tu repositorio. También puedes habilitar actualizaciones de versiones de dependencias para saber cuándo hay nuevas versiones de paquetes disponibles, para que puedas mantenerlo actualizado incluso si no se ha identificado una vulnerabilidad explícita.

- **Secretos:** Si bien deberías estar usando un administrador de secretos como se describió anteriormente, todos cometemos errores y algunos tokens pueden pasar por alto y estar incrustados directamente en el código. Las herramientas de escaneo de secretos, proporcionadas tanto a través de integraciones de terceros como mediante GitHub Advanced Security para Empresas, notifican o incluso bloquean los tokens secretos a medida que se insertan en tu repositorio.

- **Vulnerabilidades Nuevas:** A medida que escribes nuevo código, es posible que accidentalmente agregues nuevas vulnerabilidades, ya sea en el código nuevo en sí o en la forma en que conectas los componentes existentes. Hay una amplia variedad de formas de escanear tu aplicación en general, algunas de las cuales dependen del lenguaje. Las empresas también pueden confiar en el escaneo de código de GitHub Advanced Security para encontrar una amplia variedad de fallos, desde inyecciones SQL hasta referencias circulares, en la mayoría de los lenguajes de programación populares.

- **SECURITY.md** y **Informes Privados de Vulnerabilidades:** Si un usuario o investigador de seguridad identifica un problema en tu proyecto, deben saber cómo informarlo de manera segura y responsable. Incluye un archivo de política de seguridad en tu repositorio para proporcionar estas pautas y ayudar a mantener la confianza de tus usuarios y la comunidad en general. También activa los informes privados de vulnerabilidades; esto permite a los investigadores de seguridad informar de manera segura cualquier vulnerabilidad que encuentren.

5. Opciones Avanzadas

Más allá de lo básico, hay una serie de opciones avanzadas que puedes aprovechar para mejorar aún más la preparación de tu repositorio para la colaboración.

- **Plantillas de Problemas:** A medida que los colaboradores utilizan tu proyecto, presentarán problemas solicitando correcciones de errores y mejoras. Por defecto, estas solicitudes serán bastante no estructuradas y es posible que debas volver a comunicarte con el creador varias veces para obtener toda la información que necesitas. Al crear algunas plantillas de problemas, puedes proporcionar orientación, definir los campos requeridos y opcionales que los usuarios verán y configurar opciones específicas que seleccionarán al abrir problemas.

- **Configuración de GitHub Codespaces:** GitHub Codespaces proporciona un entorno de desarrollo completo y configurable sobre un repositorio. Esto permite que cualquiera trabaje en tu proyecto desde cualquier lugar, sin tener que configurar un entorno local. Proporcionar un Codespace bien configurado puede facilitar mucho la contribución de otros a tu proyecto y hace que el proyecto sea menos frágil, ya que todos los desarrolladores trabajarán desde la misma configuración (eliminando el problema de "funciona en mi máquina pero no en la tuya").

- **Entornos:** Los entornos de GitHub te permiten especificar dónde deben ocurrir ciertas tareas (como implementaciones). Pueden configurarse con reglas de protección específicas, asegurando que las tareas importantes solo ocurran de manera controlada y segura.

6. Próximos Pasos / Aspectos Externos

Ahora que has configurado tu repositorio, es hora de considerar los aspectos más amplios de la colaboración, incluido tu papel como mantenedor y cómo interactúas con tu comunidad.

- **Capacidad de Respuesta:** Como mantenedor, tu capacidad de respuesta juega un papel crucial para fomentar un entorno colaborativo saludable. Esto implica abordar rápidamente los problemas y las solicitudes de extracción, proporcionar comentarios y guiar a los nuevos colaboradores. Establece momentos específicos cada semana en los que te dediques a responder a cambios y solucionar problemas. Si quieres medir la capacidad de respuesta de tu proyecto, verifica la Acción de Métricas.

- **Gestión de Proyectos:** Las capacidades nativas de planificación de proyectos de GitHub han evolucionado enormemente y son utilizables tanto para proyectos individuales como para colaboración en toda la empresa. Configura Proyectos de GitHub para gestionar tu trabajo y proporcionar visibilidad a tu comunidad. Esto no solo te ayuda a mantener la

 organización, sino que también les brinda a los colaboradores una visión clara de lo que está en progreso y lo que está planeado para el futuro.

- **Comunicación:** A medida que tu proyecto crece, la comunicación se vuelve más importante. Utiliza las discusiones para conversaciones más largas o temas de alto nivel que no pertenecen a los problemas o solicitudes de extracción. Mantén un canal de chat como Slack o Discord para conversaciones en tiempo real y preguntas rápidas. También considera mantener una lista de correo o boletín para mantener a los interesados informados sobre los desarrollos y las próximas características.

- **Agradecimientos y Reconocimientos:** Asegúrate de reconocer y agradecer a los colaboradores que han contribuido a tu proyecto. Puedes hacerlo de muchas formas, desde destacar sus contribuciones en tu README, hasta ofrecer insignias de reconocimiento en función de sus aportaciones.

- **Crecimiento:** A medida que más personas contribuyan a tu proyecto, es importante estar preparado para el crecimiento. Esto podría incluir la formación de un equipo central de mantenimiento, la adopción de herramientas más avanzadas o la consideración de cómo escalar los recursos en función de la creciente demanda.

En resumen, preparar tu repositorio para la colaboración requiere un enfoque holístico que abarque desde la configuración hasta la automatización y la seguridad. Al seguir los pasos descritos en esta guía, estarás en una posición sólida para construir una comunidad activa de colaboradores y garantizar el éxito y la calidad de tu proyecto a lo largo del tiempo. ¡Buena suerte en tu viaje de colaboración en GitHub!TLDR, or you’ve been GitHubbing for a while? Skip to the end for a printable checklist which you can use to ensure that you've covered all aspects of making your repository collaboration-ready.



My daughter has a pair of pet gerbils. They’re awesome, but not the most complex creatures to care for. They need their cage cleaned occasionally, their food and water refilled, and may need a neighbor to check in on them if we’re away for a while. But someday, she may have a pet that requires more care and attention – a cat or dog perhaps, which needs to be played with and nurtured every day – so she’ll want to have a few good friends who know her pet and can be their companion whenever she’s away. And someday, she may even have a child of her own, making her connections to community and family ever more important. As the saying goes, it takes a village to raise a child.

So it goes with code projects. My colleagues and I often refer to our projects as “pets” or even “children” (sometimes jokingly, sometimes obsessively). We pour a lot of our own care and attention into them, but it can be easy to forget how important the community’s contributions can be to their success. In the world of software development, collaboration can make the difference between a brittle last-minute release and a reliable, maintainable, pain-free project. Whether you’ve been coding for a day or a decade, your colleagues are there to help strengthen your work. But they can only help if you’ve given them the tools to do so.

Your primary responsibility as the creator or maintainer of a repository is to ensure that others can appropriately use, understand, and even contribute to the project. GitHub is here to support that mission, but ensuring that a repo is collaboration-ready takes a bit more effort than using git clone. So read on to learn the settings, content, and behaviors that’ll help you succeed.


1. Repository Settings

The settings of your repository lay the foundation for collaboration. They determine who can see and contribute to your project, how contributions are reviewed, and what happens to those contributions once they are submitted. Properly used, they can foster an environment in which contributors across the globe will find, make use of, and help build your project. In a corporate setting, they help shift developers from a siloed way of thinking/building to a “search-first, collaborate-first” mindset. This practice, known as innersourcing, reduces redundant work and accelerates the whole company.


Visibility
You’re aiming to maximize contributions and reuse, but doesn't always mean making your repo public, especially in a corporate setting where information privacy is a consideration. You have several options available in the “Settings” tab of your repository:

Public lets anyone in the world see and copy your code, and generally allows them to create Issues or Pull Requests, so they can provide feedback about whether it works well, or even suggest (but not force) changes to improve it. This is generally great for personal projects containing no protected information (those tokens are all stored separately, right?) but only for certain “blessed” company projects.
Internal is a special visibility level used by GitHub Enterprise, allowing anyone inside your organization to see the repo, but nobody in the outside world. We generally suggest this as the default level for company projects which don’t have siloed sensitive information (e.g. customer-specific data or logic that only a specific group should know about).
Private is the most restrictive option, and can be a collaboration-killer. Use this option sparingly, and if you do, be sure to invite some…
Collaborators are specific individuals or teams you invite to be part of your project. They can be given specific roles such as “Read” (allowing them to see your otherwise private repo), “Write” (letting them directly commit or manage Pull Requests), “Admin”, and many others.

Protect the main branch
While you want to maximize the number of people who can see and contribute to your project, you still need to ensure that their contributions are properly reviewed, both by your core team members and by automation. In most cases, you’ll want to create a repository rule (the modern replacement for branch protection) on your main branch, and configure it to require a pull request before merging is allowed. By requiring at least one approver, ideally one from your CODEOWNERS file (discussed in the next section), you’ll guarantee that another human reviews each set of changes. In addition, you will want to have automated tools such as unit tests run against each pull request; these are known as status checks and will be covered under “automation/checks” below.




2. Repository Contents

Software projects don’t just consist of code. Your repository should act as a guide to collaborators, letting them know why it exists, how to use it appropriately, and the best ways to contribute. Adding a few key files (generally written using markdown) will help other people discover your project and understand how to collaborate effectively:

README.md: This is the first file visitors to your repo will see, so it is critical to include in your repository. It should describe what your project does, how to use the repo, and any configuration needed. Additionally, a good README includes the mission of the project, what it aims to do, and why it exists. Lastly, be sure to describe how and by whom the project is maintained.

LICENSE.md: A license file defines what others can and can't do with your code and other content. Whether your goal is to allow unrestricted use of your project, or to add special restrictions on its usage and distribution, it's crucial to include a license. Visit choosealicense.com for guidance on which license might work best for your project, then add one to your repository.

CONTRIBUTING.md: You can reduce the amount of confusion and friction that potential contributors (and you) face by clearly defining why and how others can contribute new code, documentation, art, or other elements to your project. If the contribution steps are very simple, you might just include them in your readme; but if you find it takes more than a paragraph or two (and it usually does), it’s best to create this separate file. It should include information about the types of contributions you're looking for, how to propose a new feature or bug fix, the process for submitting pull requests, and any specific coding standards or style guidelines contributors should follow. For a good example, take a look at the contributor guide from GitHub’s docs project.

CODEOWNERS: A CODEOWNERS file assigns one or more users who will be responsible for code in a particular part of your repository. As specified in the repository settings, these individuals will be automatically requested for review when someone opens a pull request that modifies code they own. Note that this file, unlike the others mentioned here, should not have the “.md” extension.

CODE_OF_CONDUCT.md: A code of conduct establishes the social norms, rules, and responsibilities that participants in your project should follow. It promotes a friendly and respectful environment for collaboration, and it is easy to add manually or by using one of GitHub’s templates!

With these files in place, your repository will be much more approachable and understandable, and you should start seeing contributions flow more freely. But if you want to go even further, there’s even more you can do to set up your project for healthy contributions.


3. Automation and Checks



It’s time to enter the Matrix. As Agent Smith is fond of saying, “Never send a human to do a machine's job”. While you generally want at least one human reviewer for each major change, you should make their job as easy as possible. GitHub’s built-in automation and CI/CD system, GitHub Actions, allows you to run workflows in response to file changes, pull requests, external triggers such as chat tools, and even as cron jobs. Let's look at a few ways this can make collaborators’ lives easier:


Linting
Linters are tools that analyze code to detect various types of errors and enforce a consistent coding style. Incorporating linters into your development process can greatly improve the readability and quality of your code, making it easier for others to understand and contribute to your project. One of the most popular is super linter, which can be initially configured in a single cut-and-paste step.

Building & Testing
While the exact compilers and test suites you run will be specific to the language and framework of your application, most can be executed automatically in your repo. To find the right ones, search through GitHub Marketplace’s list of Build and Test Apps & Actions, then follow the instructions specific to your preferred tool. Or, execute them by running command-line scripts and arguments in your GitHub Actions workflow.

Checks
When information is surfaced to reviewers right inside the pull request, it makes their job faster and easier, eliminating the need for them to manually run test suites or run through a physical checklist. If the automated checks fail, we can even block deployments from going out the door. Once you’ve added a linter or test suite as described above, and it has run at least once, consider configuring it as a status check in your repository settings. This will help ensure that your app is properly tested each and every time a pull request is created.

This is not a complete list, but every project is different, so also consider what other code quality, dependency management, or pre-release automation you might want to include. Then, consider how you want to deploy the project. In most cases, you’ll find there is a component in the GitHub Marketplace which provides turnkey integration with your favorite infrastructure provider, but it’s also possible to write your own GitHub Action to deploy your app after all the checks have passed. And, for high-volume enterprise projects, consider using merge queues if you start getting traffic jams on rapidly changing branches.

With these automation tools and checks in place, you can have more confidence in the quality and consistency of contributions to your repository, and spend less time manually managing the process.


4. Security



Security is a paramount concern in any software project, and especially important when including a variety of collaborators who may have different levels of security training (or none at all). Fortunately, there are a few simple steps you can take to protect your code, data, and users from potential threats.

Roles
Carefully decide which roles, and thus permissions, you give to collaborators in your repository. Generally speaking, you’ll want to assign the “Read” role to the general public. “Triage” and “Write” are for trusted individuals such as members of your company or working group (but only once protected branches and checks have been set up).  “Maintain” and “Admin” roles are best for your core maintainers, who are responsible for reviewing and managing what goes into production. Also consider that “Triage” and above have the ability to manage issues, discussions, and comments – so you’ll want to trust that they have the commitment and background to manage the flow of metadata surrounding your project. Enterprise customers can take advantage of custom repository roles, for more granular permissions control.

Secrets Management
Secrets are sensitive data like API keys, passwords, and certificates that you need to keep private. You don’t want these to be directly embedded into your code or your logs; instead, you should use either a third-party keystore or GitHub’s native secret-management tools, which can be found under the “Secrets and Variables” section of your repository settings. There, you’ll find separate sections for GitHub Codespaces (a tool described in the “Advanced Options” section below) and for GitHub Actions, because you may want to use different secrets during development than you do in production.

Security Scanners
Scanning code for vulnerabilities is a complex topic, but breaks down into three major categories:
Dependencies: 80-90% of most applications’ code comes from third-party sources – the frameworks and packages we build the rest of our code on top of. GitHub Dependabot is available on all public repositories, and can be automatically enabled in across entire organizations. It is able to alert you (and help provide a fix) whenever an insecure dependency is found. To ensure that Dependabot is running, check the “security” tab at the top of your repo. You can also enable dependency version updates to let you know when new versions of packages are available, so you can keep up-to-date even if an explicit vulnerability has not been identified.
Secrets: While you should already be using a secret manager as described above, we all make mistakes, and some tokens may slip through the cracks and get embedded directly into code. Secret scanning tools, provided both through third-party integrations and via GitHub Advanced Security for Enterprises, notify or even block secret tokens as they are pushed into your repository.
Novel Vulnerabilities: as you write new code, you may accidentally add new vulnerabilities, either in the novel code itself or in the way you wire together existing components. There are a wide variety of ways to scan your overall application, some of which are language-dependant. Enterprise can also rely on GitHub Advanced Security’s code scanning to find a wide variety of flaws, from SQL injection to circular references, in most popular coding languages. 

SECURITY.md  & Private Vulnerability Reporting
If a user or security researcher identifies a problem with your project, they need to know how to securely and responsibly report it. Include a security policy file in your repository to provide these guidelines, and help maintain the trust of your users and the wider community. Also turn on private vulnerability reporting; this allows security researchers to securely report any vulnerabilities they find! 


5. Advanced Options



Beyond the basics, there are a number of advanced options you can leverage to further enhance your repository's collaboration readiness.

Issue Templates
As collaborators make use of your project, they will file Issues asking for bug fixes and enhancements. By default, these requests will be fairly unstructured, and you may need to loop back to the creator several times to get all the information you need. By creating a few Issue Templates, you can provide guidance, define which required and optional fields users will see, and set up specific options they’ll select when opening issues.

GitHub Codespaces Config
GitHub Codespaces provides a complete, configurable dev environment on top of a repo. This allows anyone to work on your project from anywhere, without having to set up a local environment. Providing a well-configured Codespace can make it much easier for others to contribute to your project, and makes the project less brittle since all developers will be working from the same configuration (eliminating the “it works on my machine but not yours” problem).

Environments
GitHub Environments let you specify where certain tasks (like deployments) should happen. They can be configured with specific protection rules, ensuring that important tasks only happen in a controlled and secure manner.


6. Next Steps / Externalities

Now that you've set up your repository, it's time to consider the broader aspects of collaboration, including your role as a maintainer and how you engage with your community.

Responsiveness
As a maintainer, your responsiveness plays a crucial role in fostering a healthy collaborative environment. This involves promptly addressing issues and pull requests, providing feedback, and guiding new contributors. Set aside specific times each week that you’ll dedicate toward responding to changes and remediating problems. If you want to measure how responsive your project is, check out the Metrics Action.

Project Management
GitHub’s native project planning capabilities have evolved massively, and are usable both for individual projects and enterprise-wide collaboration. Set up GitHub Projects to manage your work and provide visibility to your community. This not only helps you stay organized, but also allows others to understand the current status of the project and where they can contribute.

Visibility
A well-maintained repository is of little use if nobody knows about it. Promote your project through blog posts, demos, or even dedicated project portals. The more people who know about your project, the more potential contributors and users you can attract.

Community Engagement
Engaging with your community is key to fostering a healthy collaborative environment. This might involve organizing meetups, running a project blog, or even just actively participating in discussions.

By following these standards, you can ensure that your repository is not just collaboration-ready, but also a place where a vibrant community can flourish! Print out this checklist, and use it to help guide you along each time you create (or revisit) a GitHub repository!


Is Your Repository Collaboration-Ready?

Print this checklist and use it as a guide when setting up your GitHub repositories for collaboration. Read more at gh.io/collab-ready-repo

1. Repository Settings
set appropriate repository visibility (public or private)
configure branch protection rules

2. Repository Contents
create an informative README.md
add a LICENSE.md file
include CONTRIBUTING.md
set up CODEOWNERS
establish a CODE_OF_CONDUCT.md

3. Automation/Checks
implement code linting
set up tests / Continuous Integration (CI)
configure status checks
consider Continuous Deployment (CD)
(enterprises) configure Merge Queues

6. Security
assign appropriate roles/permissions
manage secrets securely
set up scanners for dependencies, secrets, general vulnerabilities
consider Dependabot version updates
provide a SECURITY.md & enable Private Vulnerability Reporting

7. Advanced Options
add Issue Templates
configure GitHub Codespaces
define Environments

8. Next Steps / Externalities
commit to being responsive
use GitHub Projects and Issues for project management
promote your project for visibility
engage with your community
