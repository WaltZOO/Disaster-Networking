# Guidelines for LoRa Deployment in Small Urban Environments (TaillePetiteUrbExt)

## Objective

This guide provides detailed instructions for deploying a mesh LoRa network in a small urban environment. The goal is to ensure resilient communication without relays, even in the event of a natural disaster.

## Recommended Equipment

- **Frequency**: 433 MHz (for better obstacle penetration in dense urban areas).
- **Endpoints**: 4x T-BEAM Supreme (Lyligo).

## Antenna Configuration

- **Antenna Height**: Install antennas at a height of 10 meters (approximately 3 floors) to maximize range and signal quality.
- **Network Topology**: Position endpoints to create a mesh network where each node can communicate with multiple others, ensuring natural redundancy.

## Protocol and Firmware

- **Protocol**: Use the Meshtastic protocol, an automatic mesh protocol working with LoRa technology.
- **Flashing the Boards**: Use the web flasher to update the T-BEAM Supreme with the latest version of Meshtastic.

## Testing and Validation

- **Range Tests**: Conduct range tests to verify that antennas at 10 meters provide sufficient coverage in dense urban areas without requiring relays.
- **Penetration Tests**: Ensure the 433 MHz signal effectively penetrates urban obstacles.
- **Redundancy Tests**: Simulate node failures to confirm the mesh network remains functional due to redundancy.

## Conclusion

By following these guidelines, you can deploy a resilient and mesh LoRa network in a small urban environment, capable of maintaining communication even during a natural disaster, without the need for relays.

---

This guideline file is based on test results and recommendations provided in the project report. For more details, refer to the decision tree and associated test files.