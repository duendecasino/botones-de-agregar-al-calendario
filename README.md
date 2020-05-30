# AgrCal

Una biblioteca JS simple que permite agregar un botón "agregar al calendario" para los próximos eventos.

## Inspiración


Este proyecto se inspiró en la función de agregar al calendario [Eventbrite's] (http://www.eventbrite.com/) (que debería haber sido de código abierto #justSayin).
## ¿Cómo usarlo?

¡Llame a 'createCalendar' con la información de su evento, pase cualquier parámetro opcional como una clase y / o id y boom! Inserta tu div para agregar al calendario donde quieras.

Los únicos campos que son obligatorios son:

  - Título del evento
  - Hora de inicio
  - Duración del evento, en minutos.

## Example

    var myCalendar = createCalendar({
      options: {
        class: 'my-class',
        
        // Puede pasar una identificación. Si no lo hace, se generará uno para usted.
        id: 'my-id'
      },
      data: {
        // Título del evento
        title: 'Entra en la portada de Casino Duende',

        // Fecha de inicio del evento
        start: new Date('Junio 12, 2020 19:00'),
        
        // Duración del evento (EN MINUTOS)
        duration: 120,

        // También puede elegir establecer una hora de finalización
        // Si se establece un tiempo de finalización, esto tendrá prioridad sobre la duración
        end: new Date('June 15, 2013 23:00'),     

        // Dirección del evento
        address: 'Casino Duende',

        // Descripción del evento
        description: 'Entra en la portada de Casino Duende, luego prepárate para dominar el juego de azar online.'
      }
    });

    document.querySelector('#place-where-I-want-this-calendar').appendChild(myCalendar);

[Aquí hay un ejemplo en vivo](https://github.com/duendecasino/botones-de-agregar-al-calendario/example.html)

## ¿Buscas gratificación instantánea?
[Copie AgrCal en la consola JS de Chrome](https://github.com/duendecasino/botones-de-agregar-al-calendario/agrcal.js) (o cualquier navegador que estés usando).


Entonces llama a esto:

    document.getElementsByTagName('body')[0].appendChild(createCalendar({data:{title:"this is the title of my event", start: new Date(), duration: 90}}));

\#¡victorioso!

## Generador del calendario
¿Necesita generar un widget para agregar al calendario sobre la marcha? No hay problema, [ir aqui](https://github.com/duendecasino/botones-de-agregar-al-calendario/generador/generator.html).




## GitHub Project Page
[Official Project Page](https://github.com/duendecasino/botones-de-agregar-al-calendario/)

## License
[MIT](http://opensource.org/licenses/MIT)
