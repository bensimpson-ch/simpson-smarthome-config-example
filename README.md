# Simpson Smart Home Configuration Example

This repository contains example configuration files for setting up a smart home system using GitOps principles. The system supports communication over Zigbee and Matter protocols, with Docker containers running on a Raspberry Pi, and includes cloud integration with Kafka running on Microsoft Azure.

## Project Overview

This example setup demonstrates how to configure and deploy the following components:
- **Zigbee Communication** via the **Sonoff Zigbee 3.0 USB Dongle Plus**
- **Matter Communication** via the **nRF52840 USB Dongle**
- **Dockerized Services** including:
  - Custom Zigbee/Matter Processor
  - Kafka Processor
  - Apache Kafka (v3.8+)
- **GitOps Workflow** using ArgoCD for automated deployments
- **Azure Cloud Integration** with Kafka running in the cloud

## Architecture

The system runs on a **Raspberry Pi 5** and utilizes the following components:

- **Docker**: Containerized services are deployed via Docker.
- **ArgoCD**: Manages GitOps-based deployments by pulling configurations from this repository.
- **Zigbee**: The **Sonoff Zigbee 3.0 USB Dongle Plus** handles Zigbee communication.
- **Matter**: The **nRF52840 USB Dongle** handles Thread and Matter communication.
- **Apache Kafka**: Both local and cloud Kafka processors are used for data communication.
- **Azure**: Kafka is deployed in Azure using Terraform or GitHub Actions.

## Repository Structure

TBD
