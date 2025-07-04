# Project 18 - Disaster Networking with LoRa

After the passage of Chido Cyclone over Mayotte, 51 out of 54 mobile network antennas were rendered inoperable, mainly due to lack of power, thus preventing both the authorities and the population from communicating to organize rescue efforts.

Disaster Networks are communication infrastructures or systems designed to ensure connectivity and critical communications during emergency situations or natural, technological, or human-made disasters. These networks play a vital role in coordinating rescue operations, alerting populations, and restoring communications in heavily disrupted environments.

In this project, you will first compare two mesh network technologies with [LoRa endpoints](matos.md) (433 MHz, 868 MHz and 2.4 GHz):

* [ClusterDuck protocol](https://clusterduckprotocol.org/)
* [Meshtastic protocol](https://meshtastic.org/)

You will port those mesh technology stack on new [LoRa endpoints](matos.md).

You will also try to implement new message formats such as [Emergency Warning Satellite Services (EWSS)](https://gricad-gitlab.univ-grenoble-alpes.fr/Projets-INFO4/24-25/09/docs/-/blob/main/README.en.md?ref_type=heads) over Meshtastic/LoRa if you have time.

You will also try to implement [Bundle](https://datatracker.ietf.org/doc/rfc9171/) (a DTN protocol) over LoRa if you have time.

Your developments may contribute to both of these open-source communities (Meshtastic, RIOT OS ...).

## Testbeds

Field tests will be conducted using helium-filled tethered balloons on the SMH campus in the spring of 2025.

Field tests may also be conducted aboard [CNES stratospheric balloons](https://gricad-gitlab.univ-grenoble-alpes.fr/thingsat/public/-/blob/master/balloons/README.md) in Spring 2025.

![Infra 4G de Mayotte](https://air.imag.fr/images/4/42/Cartoradio-mayotte-01.jpg)

