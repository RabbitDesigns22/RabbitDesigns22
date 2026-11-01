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

Con tantos chats juntos me topé con dos problemas: gastaban tokens rehaciendo trabajo y se equivocaban de fecha. Para cada uno hice una skill, y aquí las dejo abiertas para que las uses en tu Claude Code.

### [one-pass](https://github.com/RabbitDesigns22/one-pass): bien a la primera

Lo que más tokens gasta un agente no es hablar de más. Es rehacer: entrega, se lo regresas, lo vuelve a hacer, relee los mismos archivos, repite el mismo comando que ya falló. one-pass le cambia la forma de trabajar:

- Antes de empezar, escribe en 5 líneas qué tiene que cumplir el resultado para que lo aceptes a la primera, y antes de decir "listo" lo revisa contra esa lista.
- Lee cada archivo una sola vez y apunta lo que sacó. No vuelve a abrir lo que acaba de escribir.
- Si el mismo intento falla dos veces, para, busca la causa y cambia de camino. No hay tercer intento a ciegas.
- Cuando le pasa trabajo a otro agente, le manda todo en un solo mensaje: rutas, qué evitar y cómo se ve terminado.
- Nunca se salta pruebas, confirmaciones ni revisiones para ahorrar.

Son puras instrucciones, sin scripts. No se conecta a internet ni pide permisos.

### [hora-exacta](https://github.com/RabbitDesigns22/hora-exacta): que no se pierda en el tiempo

Claude no tiene reloj. Si adivina la fecha, programa una publicación el día que no era o escribe "mañana" cuando ya pasó. Con esta skill, cada mensaje que le mandas le llega con:

- la fecha y la hora reales en CDMX, Lima, Costa Rica, Caracas y Florida (Florida ya con su cambio de horario);
- la semana en curso, de lunes a domingo;
- la ciudad aproximada según tu IP y el huso horario de tu computadora, por si viajas.

Es un script de Python sin paquetes extra. Consulta la IP como mucho cada 6 horas, y con `--sin-ip` no se conecta a nada.

### Instalar

```bash
npx skills add RabbitDesigns22/one-pass -g -y
npx skills add RabbitDesigns22/hora-exacta -g -y
```

hora-exacta pide un paso más: pegar un hook en tu `settings.json` para que la hora llegue sola. En [su página](https://github.com/RabbitDesigns22/hora-exacta#instalar-2-pasos) está cómo hacerlo, en Mac, Linux y Windows.

## ¿Tienes un negocio?

Hacemos anuncios para que te escriban por WhatsApp, páginas web que traen clientes y apps a la medida. Escríbenos desde [rabbit-designs.com](https://rabbit-designs.com).
