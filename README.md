<h1 align="center">Hola, soy Eduardo</h1>

<p align="center">
  Soy venezolano y vivo en Puebla, México. Tengo una agencia, <a href="https://rabbit-designs.com">Rabbit Designs</a>, y la saco adelante desde mi casa con un equipo de chats de Claude.<br>
  Hacemos anuncios de Meta y Google, contenido, páginas web y apps para negocios de México, Perú, Costa Rica y Venezuela.
</p>

<p align="center">
  <a href="https://rabbit-designs.com"><img src="https://img.shields.io/badge/Web-rabbit--designs.com-111111?style=for-the-badge" alt="Web"></a>
  <a href="https://www.instagram.com/rabbitdesigns.art/"><img src="https://img.shields.io/badge/Instagram-rabbitdesigns.art-E4405F?style=for-the-badge&logo=instagram&logoColor=white" alt="Instagram de Rabbit Designs"></a>
  <a href="https://www.instagram.com/addelis1988/"><img src="https://img.shields.io/badge/Mi%20historia-@addelis1988-833AB4?style=for-the-badge&logo=instagram&logoColor=white" alt="Mi Instagram personal"></a>
</p>

---

## Cómo trabajo

Tengo más de 15 chats de Claude abiertos todo el día, y cada uno tiene su trabajo:

- Cada cliente tiene su chat. Ese chat le diseña los posts, las historias y los videos de la semana para sus anuncios de Meta.
- Un chat supervisor reparte las órdenes y revisa cada pieza antes de que salga. Si algo no llega a 9 de 10, se lo devuelve al chat que la hizo.
- Un planificador programa todo en Facebook e Instagram.
- Otros chats hacen páginas web, revisan campañas de Google Ads, cuidan las apps o estudian el negocio de cada cliente.
- Algunas tareas corren solas de madrugada. Si pasa algo urgente, me avisa un bot por Telegram, con voz.

Yo casi solo hablo con el supervisor, y él les pasa el trabajo a los demás.

## Skills que comparto

Con tantos chats juntos me topé con problemas reales: gastaban tokens rehaciendo trabajo, se equivocaban de fecha, me mandaban a hacer cosas que ellos podían hacer, me daban reportes viejos y no sabían lo que hacía el chat de al lado. Para cada problema hice una skill y aquí las dejo abiertas para tu Claude Code. Casi todas son solo instrucciones (hora-exacta, skill-harvest y session-watchdog traen scripts cortos de Python), en inglés y en español, con licencia MIT.

| Skill | El problema que resuelve |
|---|---|
| [one-pass](https://github.com/RabbitDesigns22/one-pass) | Bien a la primera: deja de gastar tokens rehaciendo, releyendo y reintentando a ciegas |
| [hora-exacta](https://github.com/RabbitDesigns22/hora-exacta) | Cada mensaje llega con la fecha y la hora reales; no programa nada en el día equivocado |
| [hands-on](https://github.com/RabbitDesigns22/hands-on) | El agente hace él todo lo que puede y solo te pide lo que de verdad no puede (códigos, claves, pagos) |
| [easy-for-them](https://github.com/RabbitDesigns22/easy-for-them) | Cuando una persona tiene que hacer algo: enlace directo, una acción por línea, mensaje listo para reenviar |
| [one-answer](https://github.com/RabbitDesigns22/one-answer) | Una sola respuesta ya pensada, en vez de plan, corrección y otro plan |
| [never-twice](https://github.com/RabbitDesigns22/never-twice) | Un registro de errores compartido para que el mismo error no pase dos veces |
| [report-now](https://github.com/RabbitDesigns22/report-now) | Si pides un reporte, lo revisa en vivo en ese momento y le pone la hora; nunca uno viejo |
| [sort-me-out](https://github.com/RabbitDesigns22/sort-me-out) | "Ordéname": una lista de lo pendiente, lo bloqueado y lo que se te olvidó |
| [in-the-loop](https://github.com/RabbitDesigns22/in-the-loop) | Varios chats, un tablero en vivo: todos saben qué cambió sin meterse en el trabajo del otro |
| [small-budget-ads](https://github.com/RabbitDesigns22/small-budget-ads) | Reglas para decidir qué anuncio de Meta apagar cuando el presupuesto es chico (1 a 5 dólares al día) |
| [study-first](https://github.com/RabbitDesigns22/study-first) | Que estudie a fondo lo que pediste y lea completo antes de responder: punto por punto, sin inventar detalles |
| [session-watchdog](https://github.com/RabbitDesigns22/session-watchdog) | Despierta solo a los chats que se quedaron pegados a medias; a los que terminaron no los toca |
| [skill-harvest](https://github.com/RabbitDesigns22/skill-harvest) | Lee todos tus chats y encuentra las skills que te faltan o que tus chats olvidan cargar |
| [whatsapp-number-onboarding](https://github.com/RabbitDesigns22/whatsapp-number-onboarding) | Conecta el WhatsApp de un cliente a la API de Meta en el orden seguro, con los códigos de error reales |
| [published-vs-planned](https://github.com/RabbitDesigns22/published-vs-planned) | Solo dice "publicado" de lo que vio en vivo en la página pública; Facebook e Instagram por separado |
| [source-every-fact](https://github.com/RabbitDesigns22/source-every-fact) | Cada precio, teléfono y nombre de un post sale de su fuente; nada inventado |
| [only-what-was-asked](https://github.com/RabbitDesigns22/only-what-was-asked) | "Solo pausa Google Ads" pausa solo Google Ads, y comprueba que nada más se movió |

### Instalar

Cada una se instala con una línea. Por ejemplo:

```bash
npx skills add RabbitDesigns22/one-pass -g -y
npx skills add RabbitDesigns22/hands-on -g -y
npx skills add RabbitDesigns22/report-now -g -y
```

hora-exacta pide un paso más: pegar un hook en tu `settings.json` para que la hora llegue sola. En [su página](https://github.com/RabbitDesigns22/hora-exacta#instalar-2-pasos) está cómo hacerlo, en Mac, Linux y Windows.

## ¿Tienes un negocio?

Hacemos anuncios para que te escriban por WhatsApp, páginas web que traen clientes y apps a la medida. Escríbenos desde [rabbit-designs.com](https://rabbit-designs.com).
