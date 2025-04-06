# Guidelines for LoRa Deployment in Medium-Sized Urban Environments with Extensions (TailleMoyenneUrbExt)

## Objective

This guide provides detailed instructions for deploying a mesh LoRa network in a medium-sized urban environment with possible extensions. The goal is to ensure resilient communication, even in the event of a natural disaster.

## Recommended Equipment

- **Frequency**: 433 MHz (for better obstacle penetration in dense urban areas).
- **Endpoints**: 4x T-BEAM Supreme (Lyligo).

## Antenna Configuration

- **Antenna Height**: Install antennas at a height of 10 meters (approximately 3 floors) to maximize range and signal quality.
- **Positioning**: Position endpoints to create a mesh network where each node can communicate with multiple others, ensuring natural redundancy.

## Network Topology

- **Mesh Topology**: Use a mesh topology where each endpoint can communicate directly with multiple other endpoints.

## Protocol and Firmware

- **Protocol**: Use the Meshtastic protocol, an automatic mesh protocol working with LoRa technology.
- **Flashing the Boards**: Use the web flasher to update the T-BEAM Supreme with the latest version of Meshtastic. For other boards, follow the provided documentation to flash the Meshtastic firmware.

## Testing and Validation

- **Range Tests**: Conduct range tests to verify that antennas at 10 meters provide sufficient coverage in dense urban areas.
- **Penetration Tests**: Ensure the 433 MHz signal effectively penetrates urban obstacles.
- **Redundancy Tests**: Simulate node failures to confirm the mesh network remains functional due to redundancy.

## Conclusion

By following these guidelines, you can deploy a resilient and mesh LoRa network in a medium-sized urban environment, capable of maintaining communication even during a natural disaster.

---