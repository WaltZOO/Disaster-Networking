# Guidelines for LoRa Deployment in Small Mixed Environments with Extensions (TaillePetiteMixteExt)

## Objective

This guide provides detailed instructions for deploying a mesh LoRa network in a small mixed environment with possible extensions. The goal is to ensure resilient communication, even in the event of a natural disaster.

## Recommended Equipment

- **Frequency**: 868 MHz (for better range in open environments).
- **Endpoints**: 4x T-BEAM Supreme (Lyligo).
- **Relays**: 1x WiFi LoRa 32 (Heltec) or 1x Wio-WM1110 (if the area exceeds 3.1 km²).

## Antenna Configuration

- **Antenna Height**: Install antennas at the top of the mountain to optimize coverage in a mixed environment.
- **Positioning**: Position endpoints to create a mesh network where each node can communicate with multiple others, ensuring natural redundancy.

## Network Topology

- **Mesh Topology**: Use a mesh topology where each endpoint can communicate directly with multiple other endpoints. Use relays to extend coverage if the area exceeds 3.1 km².

## Protocol and Firmware

- **Protocol**: Use the Meshtastic protocol, an automatic mesh protocol working with LoRa technology.
- **Flashing the Boards**: Use the web flasher to update the T-BEAM Supreme with the latest version of Meshtastic. For other boards, follow the provided documentation to flash the Meshtastic firmware.

## Testing and Validation

- **Range Tests**: Conduct range tests to verify that antennas at 5 meters provide sufficient coverage in mixed areas.
- **Penetration Tests**: Ensure the 868 MHz signal offers optimal range in an open environment.
- **Redundancy Tests**: Simulate node failures to confirm the mesh network remains functional due to redundancy.

## Conclusion

By following these guidelines, you can deploy a resilient and mesh LoRa network in a small mixed environment, capable of maintaining communication even during a natural disaster.

---