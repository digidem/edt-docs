# Elección de un dispositivo

Hay una multitud de placas diferentes que se pueden usar para ejecutar EDT Offline. Desde hardware reciclado, como computadoras antiguas hasta computadoras de placa única de baja potencia.

<img src="../.gitbook/assets/pi4_rockpi_zima (1).jpg" alt="" data-size="original"> Raspberry Pi 4, Rock Pi 4, ZimaBoard

Algunas cosas importantes a tener en cuenta al elegir el dispositivo adecuado:

* Facilidad de configuración (las computadoras de placa única siempre son más fáciles)
* Precio, incluyendo la fuente de alimentación, almacenamiento, carcasa, etc.
* Rango y capacidad de WiFi
* Consumo de energía
* Poder
* Disponibilidad
* Factor de forma

#### Más fácil de configurar, pero más costoso y con menos potencia de CPU y WiFi

![Rock Pi 4 con carcasa](https://cdn.shopify.com/s/files/1/0248/6557/0909/products/DSC01592\_900x600.jpg?v=1636979793)

Las computadoras de placa única son las más fáciles de configurar. Hemos probado en Raspberry Pi 4 y Rock Pi 4, y hemos tenido excelentes resultados. El Raspberry 3 también debería ser capaz de manejarlo, pero aún no lo hemos probado.

Para todas estas placas, es cuestión de descargar la última versión del [repositorio de Github](https://github.com/digidem/edt-offline/releases/latest) y quemarlas en una tarjeta micro-SD clase 10 usando un software como [Balena Etcher](https://www.balena.io/etcher).

**Recomendado: Rock Pi 4 B+**

Recomendamos la placa [**Rock Pi 4 B+**](https://rockpi.org/rockpi4) debido a la escasez de chips en todo el mundo que resulta en una escasez de placas Raspberry Pi.

Además de la placa en sí, necesitará refrigeración, ya que las placas tienden a sobrecalentarse sin un sistema de refrigeración adecuado.

También necesitará una fuente de alimentación en caso de que no esté incluida con la placa, y es importante que sea un USB C 5v con al menos 3A.

Y finalmente necesitará almacenamiento, que debe ser al menos una tarjeta micro-SD clase 10.

**Comprar en Amazon:**

* [Rock Pi 4B](https://www.amazon.com/dp/B0B4MWBKR7?psc=1\&ref=ppx\_yo2ov\_dt\_b\_product\_details)
* [3.5A USB C fuente de alimentación](https://www.amazon.com/dp/B07TYQRXTK?psc=1\&ref=ppx\_yo2ov\_dt\_b\_product\_details)"* [Tarjeta Micro SD de 32GB, clase 10](https://www.amazon.com/dp/B07XDCZ9J3?psc=1\&ref=ppx\_yo2ov\_dt\_b\_product\_details)
* [Estuche con disipador de calor incorporado](https://www.amazon.com/dp/B0B7P41CTS?psc=1\&ref=ppx\_yo2ov\_dt\_b\_product\_details)

#### Barato, con CPU y WiFi potentes, pero más difícil de configurar

![Zimaboard con módulo Wifi PCI express](<../.gitbook/assets/zimaboard\_wifi (1).jpg>)

Cualquier computadora de escritorio o portátil vieja puede ser utilizada como dispositivo EDT sin conexión. Sin embargo, es un poco más difícil de configurar y normalmente requiere acceder al BIOS de la computadora y cambiar algunas configuraciones para establecer USB como dispositivo principal de arranque. Esto requerirá al menos un teclado y una pantalla, y los cables correspondientes para conectarlos.

Después de cambiar las configuraciones del BIOS, necesitarás grabar la imagen amd64 desde la página de [lanzamiento](https://github.com/digidem/edt-offline/releases/latest) y grabarla en una unidad USB con suficiente almacenamiento.

Apaga el dispositivo, inserta la unidad USB y enciéndelo nuevamente. Este proceso puede tardar varios minutos y puede requerir algunos reinicios, pero una vez finalizado tendrás una instancia EDT sin conexión completamente funcional.

Si vas a comprar una computadora para usar con EDT sin conexión, recomendamos mini PC como el [Intel Nuc](https://www.intel.com.br/content/www/br/pt/products/details/nuc.html).

**Recomendado:** [**ZimaBoard**](https://www.zimaboard.com/)

Es una de las placas más baratas que puedes conseguir, con el factor de forma más pequeño. Su puerto PCI express hace que sea fácil conectar diferentes adaptadores WiFi, que dependerán de qué tan rápida quieras que sea la conexión, cuántas personas puedan manejarla al mismo tiempo y qué tan lejos necesites que llegue tu punto de acceso WiFi.

**Comprar en Amazon**

* [ZimaBoard](https://www.amazon.com/dp/B0BKL4SRJT?psc=1\&ref=ppx\_yo2ov\_dt\_b\_product\_details)
* [Adaptador de WiFi PCIe](https://www.amazon.com/dp/B08J8BHBXJ?psc=1\&ref=ppx\_yo2ov\_dt\_b\_product\_details)
* [Adaptador de mini Display a HDMI](https://www.amazon.com/dp/B0134V3KIA?psc=1\&ref=ppx\_yo2ov\_dt\_b\_product\_details)

### Lista completa de posibles dispositivos

#### Computadoras de placa únicaPor lo general, debido a que utilizan CPUs ARM, tienden a consumir menos energía y tener un factor de forma más pequeño, pero son menos capaces y generalmente no incluyen almacenamiento, carcasa o un sistema de refrigeración.

* [Rock Pi 4](https://a.co/d/95OOIZM) (\~90 USD) 🇺🇸
  * 4GB LPDDR4
  * RK3399 Hexa-Core
  * Ethernet Gigabit
  * WiFi de doble banda
* [Raspberry Pi 4](https://a.co/d/iAgYwIs) (\~125 USD - \~152 USD) 🇺🇸
  * 1GB / 2GB / 4GB / 8GB LPDDR4
  * BCM2711 Quad-Core
  * Ethernet Gigabit
  * WiFi de doble banda
* [reRouter CM4 1432](https://www.seeedstudio.com/Dual-GbE-Carrier-Board-with-4GB-RAM-32GB-eMMC-RPi-CM4-Case-p-5029.html) (\~160 USD) 🇨🇳
  * Incluye carcasa y fuente de alimentación
  * 4GB LPDDR4
  * 32GB eMMC
  * BCM2711 Quad-Core
  * 2x Ethernet Gigabit
  * WiFi de doble banda
* [RockPro 64](https://pine64.com/product/rockpro64-4gb-single-board-computer/) (\~80 USD) 🇨🇳
  * 4GB LPDDR4
  * RK3399 Hexa-Core
  * Ethernet Gigabit
  * No incluye WiFi
* [ZimaBoard](https://www.seeedstudio.com/ZimaBoard-216-X86-p-5298.html) (\~120 USD - \~200 USD) 🇺🇸
  * Incluye carcasa y fuente de alimentación
  * 16GB / 32GB eMMC
  * 4GB / 8GB LPDDR4
  * Intel Celeron N3350
  * 2x Ethernet Gigabit
  * Sin WiFi, pero con 4x puertos PCIe para dongle
* [ODYSSEY-X86](https://www.seeedstudio.com/ODYSSEY-X86J4125800-p-4915.html) (\~220 USD - \~300 USD) 🇨🇳
  * 0 / 64GB / 128GB eMMC
  * 8GB LPDDR4
  * Intel Celeron J4125
  * 2x Ethernet Gigabit
  * WiFi de doble banda
  * 2x M.2 PCIe
* [Khadas VIM2](https://a.co/d/0d0TWcv) (\~89 USD - \~100 USD) 🇺🇸

    > Sin confirmar el soporte de Balena

    * 16GB / 32GB eMMC
    * 2GB / 3GB LPDDR4
    * Amlogic S912 1.5 GHz 64Bit Octa Core ARM Cortex-A53 750MHz
    * Ethernet Gigabit
    * WiFi de doble banda MIMO 🔥

#### Mini PCs sin ventilador

Suelen ser más baratos y potentes que las SBC, y vienen completos con almacenamiento, carcasa y fuente de alimentación.* [Bmax B1 Plus](https://www.amazon.com/Bmax-B1-Plus-Computer-Ethernet/dp/B0BHP34TH1/ref=sr\_1\_4?keywords=Bmax%2BMini%2BPC\&qid=1677967510\&s=electronics\&sr=1-4\&ufe=app\_do%3Aamzn1.fos.f5122f16-c3e8-4386-bf32-63e904010ad0\&th=1) (\~120 USD) 🇺🇸
  * 8GB DDR3
  * 128GB SSD
  * Intel Celeron
  * Ethernet Gigabit
  * WiFi de doble banda
* [N40](https://a.co/d/5QoK6Uw) (\~110 USD) 🇺🇸
  * 4GB DDR4
  * 64GB eMMC
  * Intel Celeron
  * Ethernet Gigabit
  * WiFi de doble banda
* [Beelink T4 Pro](https://a.co/d/9OSdXs4) (\~100 USD) 🇺🇸
  * 4GB DDR
  * 64GB eMMC
  * Intel Celeron
  * Ethernet Gigabit
  * WiFi de doble banda
* [MeLE Quieter2Q](https://a.co/d/8EMGSYe) (180 USD - 280 USD) 🇺🇸
  * 4GB - 8GB LPDDR4
  * 64GB - 512GB M.2 SSD
  * Intel Celeron
  * Ethernet Gigabit
  * WiFi de doble banda
* [AWOW](https://a.co/d/f6pVMX6) (\~130 USD) 🇺🇸
  * 4GB DDR4
  * 64GB eMMC
  * Intel Celeron
  * Ethernet Gigabit
  * WiFi de doble banda