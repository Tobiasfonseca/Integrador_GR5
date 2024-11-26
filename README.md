# Taller Integrador GR5

## Introducción

El envejecimiento de la población y el aumento en la esperanza de vida han creado una necesidad creciente de sistemas de asistencia para adultos mayores, especialmente en cuanto a la provisión de soluciones de monitoreo remoto para garantizar su seguridad y bienestar. Las tecnologías de IoT (Internet de las Cosas) presentan una gran oportunidad para abordar esta necesidad, ofreciendo dispositivos conectados que permiten el monitoreo en tiempo real y la comunicación inmediata en situaciones de emergencia. Según la Organización Mundial de la Salud, en el año 2050, una de cada seis personas en el mundo tendrá más de 65 años, lo que plantea un desafío crítico en cuanto al cuidado y la seguridad de esta población vulnerable.

Este proyecto propone el desarrollo de un sistema de alerta de emergencia para adultos mayores, utilizando tres componentes principales: un dispositivo de rastreo con botón de pánico (Tracker), un módulo de retransmisión de señal (iGate), y una aplicación móvil para la recepción de alertas por parte de los seres queridos. El diseño del sistema permite que el adulto mayor envíe una alerta rápida y directa mediante la presión de un botón en el Tracker, el cual activa la comunicación inmediata a través de redes de baja potencia, como LoRa y APRS. Estas tecnologías de comunicación son ideales para cubrir largas distancias de manera eficiente y con bajo consumo de energía, elementos críticos para asegurar la confiabilidad del sistema en situaciones de emergencia.

Una de las ventajas de este sistema es su capacidad de transmitir datos de ubicación en tiempo real mediante el uso de GPS. Al recibir la señal, el iGate procesa y retransmite la alerta, enviándola a la aplicación móvil donde los familiares del adulto mayor pueden visualizar la ubicación exacta del usuario en un mapa. La investigación muestra que el uso de plataformas IoT, junto con aplicaciones móviles de monitoreo, permite una respuesta más rápida y efectiva por parte de los familiares y cuidadores. Esto resulta especialmente útil en casos de caídas o desorientación, donde el adulto mayor puede encontrarse en lugares que le dificultan pedir ayuda.

Estudios recientes han demostrado que los sistemas de monitoreo basados en IoT son una herramienta efectiva para mejorar la calidad de vida de los adultos mayores, ya que ofrecen una mayor autonomía y reducen la preocupación de sus familiares. Sin embargo, el desarrollo de estos sistemas presenta desafíos técnicos, como la integración de múltiples tecnologías de comunicación, el consumo energético y la precisión en la localización. Para enfrentar estos desafíos, el proyecto utiliza protocolos de comunicación de baja potencia y un diseño modular que permite la adaptación y escalabilidad del sistema, asegurando su funcionalidad en distintos entornos y necesidades.

Este sistema tiene el potencial de brindar mayor seguridad y confianza a los adultos mayores, permitiéndoles mantener una vida independiente sin sacrificar su seguridad. A través de la combinación de IoT, redes de comunicación de largo alcance y aplicaciones móviles, este proyecto pretende establecer un marco de referencia para la implementación de sistemas de asistencia remota que puedan ser escalables y adaptables a las necesidades cambiantes de una población en proceso de envejecimiento.

## Diagramas
### Primer Nivel
![image](https://github.com/user-attachments/assets/fc56dd51-3f34-46b9-8901-1cbaa66f3e9c)

### Segundo Nivel
![image](https://github.com/user-attachments/assets/f1689e67-f506-42f8-9dd7-eb30ad62956f)

### Tercer Nivel
![image](https://github.com/user-attachments/assets/509e89d5-f7e3-4c68-a1b5-b577cabb7a1e)

### Cuarto Nivel
![image](https://github.com/user-attachments/assets/b5ce4510-cbb1-4ec8-9a99-258c5559a8a3)

### Quinto Nivel
![image](https://github.com/user-attachments/assets/0ea5230c-7e50-40f4-be6c-4a2b00f5d4de)

## Diagramas de flujo

### Tracker
![image](https://github.com/user-attachments/assets/6da5b414-d841-443b-a7a5-616b5b1642ea)

### iGate
![image](https://github.com/user-attachments/assets/a4243bdd-5aac-469f-87cf-5ac010a2162b)

## Configuración
En el archivo igate_conf.json dentro de la carpeta data se realizan los cambios en las siguientes líneas:

![image](https://github.com/user-attachments/assets/84d854d2-28e9-4a10-920e-1cdcbc12a5cd)
![image](https://github.com/user-attachments/assets/74a75e98-7bb2-409f-a160-2fab57f33335)

Mediante estos cambios, se configura el nombre del iGate, la conexión a internet, su localización y conexión a APRS.

### iGate configurado

![image](https://github.com/user-attachments/assets/4ff2ca93-65dd-46c3-9973-6c4c737e117a)

### iGate en el sitio APRS

![image](https://github.com/user-attachments/assets/13e90306-fb68-400f-97ad-941ab7919bea)

Basado en el repositorio de RichonGuzman:
https://github.com/richonguzman/LoRa_APRS_iGate
