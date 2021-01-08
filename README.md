# Distributed-Systems-Lab

A portfolio of production-grade engineering solutions focused on distributed systems and microservice architectures. Features high-performance gRPC frameworks, unified HTTP proxies, and scalable service interfaces designed for real-world production environments.

## 1. [http-proxy](http-proxy/) 
Microservice Unified Proxy，a lightweight proxy layer for microservices, designed to provide a consistent and unified interface across different services.
This project simplifies service integration by:
- Exposing a standardized API gateway for all microservices
- Hiding internal service complexity behind a unified proxy
- Enabling easier scaling, monitoring, and maintenance of distributed systems

## 2. [gRPC-server-interfaces](gRPC-server-interfaces/) 
This repository provides gRPC interface definitions that can be used as a shared dependency for building gRPC services or consumed by other projects.
It contains the .proto files and generated stubs required to ensure consistent communication across different services and clients.  

**Use cases**  
- As a base library for implementing new gRPC services.
- As a dependency for clients that need to call existing gRPC services.
- To maintain a unified contract for inter-service communication.

## 3. [gRPC-server](gRPC-server/) 

A lightweight and extensible gRPC server framework that implements the interfaces defined in gRPC-server-interfaces
. This project allows you to easily configure and run multiple gRPC services within a single server instance.

**Features**  

- 🔌 Interface-driven: Implements service definitions from [gRPC-server-interfaces](gRPC-server-interfaces/) .
- ⚙️ Configurable: Load and run multiple gRPC services via configuration.
- 📦 Reusable: Can serve as a base framework for new projects that need gRPC communication.
- 🚀 Extensible: Add new service implementations with minimal boilerplate.

**Use cases**  
- Build a gRPC service framework for microservices.
- Run multiple gRPC services in a single server process.
- Share the same interface contracts across different services and clients.
