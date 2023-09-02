# Sonda Multiparamétrica - UNSAM - 3ia

## Introducción
El desarrollo de instrumental de código y hardware abierto posibilita tanto la fabricación de nuevas tecnologías, así como el rediseño y adecuación de instrumentos a las necesidades propias del usuario. Esto permite el acceso libre a la documentación de diseño y funcionamiento, generando la posibilidad de que los instrumentos desarrollados puedan ser replicados, ensamblados, estudiados, modificados, compartidos y comercializados por cualquier persona de forma colaborativa. 

El presente proyecto propone el diseño de una sonda multiparamétrica de bajo costo que permita el sensado _in situ_ y remoto de variables fisicoquímicas de relevancia ambiental como la conductividad, oxígeno disuelto, temperatura y pH en cuerpos de agua. Actualmente se cuenta con el primer prototipo basado en Arduino, el cual se busca perfeccionar con el fin de lograr un producto más robusto, económico y eficiente. En este proyecto de beca se propone realizar la integración del microcontrolador a una placa única que permita adquirir datos y almacenarlos por períodos prolongados de tiempo, reducir el consumo energético y mejorar la robustez teniendo en cuenta que operará la mayor parte del tiempo en el exterior. El proyecto posee financiamiento, por lo que se facilitarán al postulante los materiales y fondos necesarios para llevarlo a cabo de manera exitosa.

<p align="center">
<img align="center" src="https://github.com/FranciscoGBianco/SondaMultiP-UNSAM/blob/main/Sonda.jpg" width="250"  height="300">
</p>

## Hardware

La estación de monitoreo consiste en una caja estanca sellada que flota asistida por boyas auxiliares, la cual en su interior contiene un microcontrolador Arduino modelo Mega, conectado a un reloj externo, un módulo de memoria SD, un módulo de bluetooth de baja energía, el sistema de alimentación basado en energía solar y los sistemas de procesamiento y desacoplamiento de las señales de cada uno de los sensores. De esta caja se extienden los sensores mediante cables sumergibles que permiten el muestreo en el agua.

En cuanto a los aspectos energéticos, se diseñó un sistema basado en energía solar. El mismo cuenta con una batería de tipo Li-Ion que alimenta al microcontrolador y a los sensores, que a su vez se encuentra conectada a un panel solar de 1 Watt, teniendo autonomía energética por tiempo indeterminado.

Además, integra un dispositivo de Bluetooth de tecnología 4.0 BLE (Bluetooth Low Energy), el cual mediante la aplicación Serial Bluetooth Terminal® permite controlar el funcionamiento de la sonda, esto es, la ejecución remota de funciones de encendido y apagado, selección de intervalo de las mediciones, calibración de sensores y consulta, curado y colección de datos. Es importante resaltar que cada medida realizada incluye la fecha y hora exactas en la que fue realizada. Estas prestaciones permiten fácilmente realizar monitoreos remotos de muchas variables relevantes durante periodos largos de tiempo, pero con altas tasas de muestreo, pudiendo obtener series temporales detalladas del sitio de estudio. 



<p align="center">
<img align="center" src="https://github.com/FranciscoGBianco/SondaMultiP-UNSAM/blob/main/Schematic_V1.0.png" width="750"  height="500">
</p>
