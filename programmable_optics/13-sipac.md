# Flexible silicon photonic architecture for accelerating distributed deep learning

## Summary
This work introduces using silicon photonics-based compute cluster to accelerate multi-tenant ML workloads through optimizing collective communication on the hardware. The hardware includes a wavelength-reconfigurable transceiver design and a wavelength-reconfigurable switch. The collective algorithm is also designed to work on the reconfigurable network fabrics. In large scale simulation, Flex-SiPAC is able to reduce the communication time by 26% to 29%.

## Pros
- Allows circuit switching in fine-granularity
- Allows optical multi-casting

## Cons
- Individual CU need multiple optical ports
- Assumes jobs are placed sequentially onto the cluster