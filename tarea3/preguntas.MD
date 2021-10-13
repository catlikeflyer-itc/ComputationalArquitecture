# Respuestas de las preguntas
1. What is the function of a CPU?

        La función principal de la CPU en el ordenador es almacenar y procesar realizando todos los cálculos matemáticos y lógicos con los datos de entrada para proporcionar los datos de salida a los usuarios. (Digital World 839, s.f.)

3. What does the control unit do?

        Controla y supervisa las comunicaciones entre el hardware conectado al ordenador, la entrada y salida de datos, comprueba que las señales se hayan entregado correctamente y se asegura de que los datos vayan al lugar correcto en el momento adecuado. (BBC, 2021)

4. Where are registers located and what are the different types?

        Los registros son memorias muy rápidas que se utilizan para ejecutar programas y operaciones de forma eficaz. El único proposito de tener registros es recuperar (leer) rápidamente los datos para su proceso en el CPU. Los diferentes tipos de registros son:

        - Acumulador: Es el registro más utilizado para almacenar datos tomados de la memoria. Se encuentra en diferentes números en diferentes microprocesadores. 
        - Registros de Dirección de Memoria (MAR): Contiene la dirección de la ubicación a la que se va a acceder desde la memoria. El MAR y el MDR (Registro de Datos de Memoria) facilitan conjuntamente la comunicación de la CPU y la memoria principal. 
        - Registros de Datos de Memoria (MDR): Contiene los datos que se van a escribir o leer de la ubicación direccionada. 
        - Registros de propósito general: Están numerados como R0, R1, R2....Rn-1, y se utilizan para almacenar datos temporales durante cualquier operación en curso. 
        - Contador de Programa (PC): El contador de programa (PC) se utiliza para mantener el seguimiento de la ejecución del programa. Contiene la dirección de memoria de la siguiente instrucción a ser obtenida. El PC apunta a la dirección de la siguiente instrucción que se obtendrá de la memoria principal cuando la instrucción anterior se haya completado con éxito. El Contador de Programa (PC) también funciona para contar el número de instrucciones. 
        - Registro de instrucciones (IR): El IR contiene la instrucción que está a punto de ser ejecutada. La instrucción del PC se obtiene y se almacena en el IR. 
        - Registro de código de condición (CCR) : Los registros de código de condición contienen diferentes banderas que indican el estado de cualquier operación.

    (GeeksForGeeks, 2020)

5. How does the ALU know which function to perform?

        La ALU realiza las operaciones lógicas, como las comparaciones, y aritméticas, como la suma y la multiplicación, necesarias durante la ejecución del programa, sabe qué operaciones debe realizar porque está controlada por las señales de la unidad de control. 

9. Explain the differences between data buses, address buses, and control buses.

        - Buses de datos: contiene la información real que debe ser movida.
        - Buses de dirección: indica la ubicación en la que deben estar los datos.
        - Buses de control: indica qué dispositivo tiene permiso para utilizar el bus y con qué propósito.

12. What is the difference between synchronous buses and nonsynchronous buses?

        - Buses sincrónicos: Todos los dispositivos están sincronizados con un reloj común. Requiere una lógica menos complicada y se ha utilizado en la mayoría de los buses existentes. Sin embargo, un bus síncrono no es fácilmente actualizable. Los nuevos procesadores más rápidos son difíciles de encajar en un bus lento.
        - Buses no-sincrónicos: Todos los dispositivos conectados al bus pueden tener diferentes velocidades y sus propios relojes. Utilizan un protocolo de handshaking para sincronizarse entre sí. Esto proporciona independencia a las diferentes tecnologías y permite que dispositivos más lentos y más rápidos con diferentes velocidades de reloj funcionen juntos. 

18. What is the difference between a byte and a word? What distinguishes each?

        La cantidad de bits que componen a un byte es de 8 bits (por lo general) y un word comunmente tiene 8, 16, 32 y 64 bits. En primera instancia su diferenciador más notorio es el hecho de que un byte es la unidad más pequeña reconocida por el CPU mientras que el word es el conjunto de bits más grande el cuál el CPU puede realizar funciones.

22. Describe how an interrupt works and name four different types.

        Como su nombre indica, los interruptores emiten una señal que interrumpe la ejecución de la CPU e inicia la ejecución de un código de interrupción específico, llamado manejador de interrupción.

        Existen dos tipos de interrupciones:

        - Software: instrucción de la CPU para interrumpirla (normalmente tiene 1 o más parámetros)
        - Hardware: un pin en la CPU que activará la interrupción

        Además de la clasificación anterior, los interruptores también pueden ser:

        - Enmascarables: pueden ser desactivadas
        - No enmascarables: siempre activadas. Normalmente se llama NMI - interrupción no enmascarable.

    (Zoric, D., 2021)

32. Explain the steps of the fetch-decode-execute cycle.

        1. El procesador comprueba el contador de programa para ver qué instrucción debe ejecutar a continuación.
        2. El contador de programa da un valor de dirección en la memoria de dónde está la siguiente instrucción.
        3. El procesador obtiene el valor de la instrucción de esta posición de memoria.
        4. Una vez obtenida la instrucción, hay que descodificarla y ejecutarla. Por ejemplo, esto podría implicar tomar un valor, ponerlo en la ALU, luego tomar un valor diferente de un registro y sumar los dos.
        5. Una vez completado esto, el procesador vuelve al contador de programa para encontrar la siguiente instrucción.
        6. Este ciclo se repite hasta que el programa termina.

    (BBC, 2021)

## Referencias
BBC. (n.d.). Fetch-decode-execute cycle - instructions - GCSE computer science revision - BBC bitesize. BBC News. Retrieved October 13, 2021, from https://www.bbc.co.uk/bitesize/guides/z2342hv/revision/5. 

BBC. (n.d.). What is the purpose of the CPU? - the CPU and the fetch-execute cycle - KS3 computer science revision - BBC bitesize. BBC News. Retrieved October 11, 2021, from https://www.bbc.co.uk/bitesize/guides/zws8d2p/revision/1. 

Different classes of CPU registers. GeeksforGeeks. (2020, December 23). Retrieved October 11, 2021, from https://www.geeksforgeeks.org/different-classes-of-cpu-registers/. 

Meyers, R. A. (2002). In Encyclopedia of Physical Science and Technology. Academic Press. 

Null, L., &amp; Lobur, J. (2003). The Essentials of Computer Organization and Architecture: Linda Null, Julia Lobur. EEUU: Jones and Bartlett. 

What is the function of CPU?, how CPU works? " CPU Basics. Digitalworld839.com. (2021, September 1). Retrieved October 11, 2021, from https://digitalworld839.com/what-is-the-function-of-cpu-and-how-cpu-works/. 