# ⏳ ¿Cómo surgieron las redes computacionales?

Las redes no nacieron para ver videos en YouTube, nacieron por dos razones principales: supervivencia y eficiencia.

Partimos de la pregunta ¿Qué sería un mundo sin redes computacionales? Debido a la necesidad de los seres humanos de comunicarse entre nosotros, lo cual nos ha permitido inventar diversas formas de hacerlo:

* #### Verbal
    Lenguaje y escritura.

* #### No verbal
    Lenguaje corporal, gestos, expresiones faciales, contacto, sonido, simbolos, visual, tacto y etc.

Por la dificultad de comunicarnos a largas distancias, hubo la necesitadad de crear formas de hacerlo.

### Señales de humo, fuego o luz

![](https://blogs.upm.es/museotelecomunicaciones/wp-content/uploads/sites/1098/2024/04/Telegrafia-con-antorchas_Grecia.jpg)

>Fuente: [Museo de Telecomunicaciones de la Universidad Politécnica de Madrid](https://blogs.upm.es/museotelecomunicaciones/comunicacion-a-distancia-inicios/)

### Servicio postal o correo

![Correo](https://www.gaceta.unam.mx/wp-content/uploads/2020/10/postal001.jpg)

>Fuente:[Universidad Nacional Autónoma de México](https://www.gaceta.unam.mx/el-correo-postal-o-electronico-esta-vivo-desde-la-antiguedad/)

### Telegrafo

![](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a9/2006_08_22_142911_Aalborg_Marinemuseum_ubt.jpeg/960px-2006_08_22_142911_Aalborg_Marinemuseum_ubt.jpeg?20060916205510)

>Fuente: [Wikipedia](https://es.wikipedia.org/wiki/Tel%C3%A9grafo)

### Código Morse

![](https://www.ambientum.com/wp-content/uploads/2024/10/codigo-morse-696x696.jpg)

>Fuente: [Ambientum](https://www.ambientum.com/ambientum/curiosidades/que-es-el-codigo-morse-y-para-que-sirve.asp)

### Teléfono

![](https://s3.amazonaws.com/s3.timetoast.com/public/uploads/photo/10555690/image/e2bfafdb7732fe2080c2cd69383f63ef?X-Amz-Algorithm=AWS4-HMAC-SHA256&X-Amz-Credential=AKIAJB6ZCNNAN7BE7WDQ%2F20260105%2Fus-east-1%2Fs3%2Faws4_request&X-Amz-Date=20260105T231415Z&X-Amz-Expires=604800&X-Amz-SignedHeaders=host&X-Amz-Signature=e800bf6c7188fd58777676e551828833f82b11dda2d57fae3065555019f8f1df)

>Fuente: [Timetoast](https://www.timetoast.com/timelines/evolucion-de-los-telefonos-celulares-d0ea2adc-7be3-4f40-81f6-d64139850ef3)

## 🔬 Hay que entender la necesidad que creó las redes computacionales

1. ### El problema inicial: "Sneakernet" (Años 50-60)

    Antes de las redes, las computadoras eran Mainframes: máquinas gigantescas que ocupaban habitaciones enteras.

    * El problema: Si querías llevar información de la Computadora A a la Computadora B, tenías que guardar los datos en una cinta magnética o tarjetas perforadas, levantarte, caminar y ponerlas en la otra máquina.

    * El concepto: A esto se le llamaba burlonamente "Sneakernet" (Red de zapatillas), porque la velocidad de transmisión dependía de qué tan rápido caminabas.

    * La necesidad: Había pocas computadoras y eran carísimas. Los investigadores necesitaban una forma de acceder a ellas remotamente sin viajar físicamente.

2. ### La Guerra Fría y la idea de ARPA (Años 60)

    En plena tensión entre EE.UU. y la Unión Soviética, el Departamento de Defensa de EE.UU. creó ARPA (Advanced Research Projects Agency).

    * El miedo: Las redes de comunicación de la época (teléfonos) usaban conmutación de circuitos. Si destruías el nodo central o cortabas un cable principal, toda la comunicación moría.

    * La solución teórica: Necesitaban una red descentralizada. Si una parte de la red era destruida (por un ataque nuclear, por ejemplo), la información debía encontrar otro camino automáticamente para llegar a su destino.

3. ### La Gran Innovación: Conmutación de Paquetes

    Esta es la piedra angular técnica. Tienes que documentar esto muy bien.

    * Antes (Circuitos): Como una llamada telefónica antigua. Se abría un canal exclusivo entre A y B. Si estaba ocupado, nadie más pasaba.

    * La Revolución (Paquetes): La información no se manda toda junta. Se "rompe" en pedacitos pequeños (paquetes).

        * Cada paquete puede tomar una ruta diferente para llegar al destino.

        * Si un camino se bloquea, el paquete toma otro.

        * Al llegar, el destino los reordena.

        Analogía para tus notas:

        * Conmutación de Circuitos: Un tren. Todos los vagones van juntos por una sola vía. Si la vía se rompe, el tren se detiene.

        * Conmutación de Paquetes: Enviar las páginas de un libro en 100 sobres diferentes por distintos camiones de correo. Si un camión se retrasa, los otros llegan, y al final tú armas el libro de nuevo.

4. ### El nacimiento: ARPANET (1969)

    El 29 de octubre de 1969 se considera el nacimiento de Internet. Se conectaron 4 nodos (universidades):

    1. UCLA (Los Ángeles)
    2. Stanford
    3. UCSB (Santa Bárbara)
    4. Universidad de Utah

    Dato curioso: El primer mensaje que intentaron enviar fue la palabra "LOGIN". Enviaron la "L", luego la "O", y el sistema colapsó. Pero habían logrado comunicarse a distancia.

5. Uniendo todo: TCP/IP (1983)

    Con el tiempo surgieron otras redes (satelitales, de radio), pero no hablaban el mismo idioma.

    * Vint Cerf y Bob Kahn crearon el protocolo TCP/IP.

    * Este protocolo permitió que redes diferentes se conectaran entre sí. Fue el momento en que ARPANET dejó de ser una sola red y se convirtió en una "Inter-Net" (Red de redes).

6. La Web para todos (1990s)

    Hasta los 90, internet era pantalla negra y texto verde, solo para científicos.

    * Tim Berners-Lee inventó la World Wide Web (WWW).

    * Creó el HTML (para hacer páginas), el HTTP (para transmitirlas) y el primer navegador. Esto hizo la red visual y accesible para cualquier persona.