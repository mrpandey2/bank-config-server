# Config Server

This repository contains the source code for the **Config Server** that serves centralized configuration to all microservices in the system. The configuration is typically managed in version control (e.g., Git) and can be dynamically updated, allowing microservices to load their configuration from a centralized location at runtime.

## Project Overview

The **Config Server** allows microservices to access and retrieve configuration properties from a central source (e.g., Git repository, file system, etc.). The server provides a REST API to expose the configurations to clients. This setup helps in managing configurations consistently across multiple environments and services.

This project is implemented using **[Spring Cloud Config](https://spring.io/projects/spring-cloud-config)** and can be extended to support other configuration management frameworks.

## Features

- Centralized management of configurations for multiple services.
- Supports Git-backed configuration storage.
- Provides dynamic configuration refresh (optional with Spring Cloud Bus or other event-driven mechanisms).
- Customizable for various configuration storage backends like Git, Vault, and file system.

## Prerequisites

- **Java 21** or higher
- **Spring Boot** 3.x
- **Spring Cloud Config** (or alternative configuration management framework)
- Docker (optional, if using containerized deployment)

## Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/mrpandey2/config-server.git
cd config-server
