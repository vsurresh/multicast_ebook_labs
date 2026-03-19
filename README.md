# Multicast eBook Labs

This repository contains [netlab](https://netlab.tools) topology files for the labs accompanying the Multicast eBook.

## What is netlab?

[netlab](https://netlab.tools) is a network infrastructure abstraction and automation tool that lets you define network topologies in simple YAML files and spin up fully configured virtual labs. It handles device provisioning, IP addressing, routing protocol configuration, and more so you can focus on the concepts.

## Required Images

The labs in this repository require the following virtual network device images:

- **Cisco IOL** — Cisco IOS image
- **Arista cEOS** — Arista cEOS image

## Spinning Up a Lab

1. Navigate to the lab directory you want to run:
   ```bash
   cd <lab-directory>
   ```

2. Start the lab:
   ```bash
   netlab up
   ```

   netlab will create the topology, configure all devices, and bring the lab online.

## Tearing Down a Lab

To stop the lab and remove all associated resources:

```bash
netlab down --cleanup
```

This removes the running containers/VMs and cleans up any generated configuration files.

## Further Reading

- [Introduction to netlab](https://www.packetswitch.co.uk/netlab-the-fastest-way-to-build-network-labs/)
