# Working with Microservices in Go

This project is a hands-on journey into building, testing, and deploying microservices using Go (Golang). It covers a wide range of essential concepts and tools needed to work with microservices architecture, from creating basic services to deploying them using Docker Swarm and Kubernetes.

---

## 🚧 What We'll Build

A front-end web application that connects to multiple microservices:

### Microservices Overview

- **Broker** – Acts as an optional single point of entry to all other microservices.
- **Authentication** – Manages user authentication and token issuance, backed by **PostgreSQL**.
- **Logger** – Centralized logging service using **MongoDB**.
- **Mail** – Sends emails using a predefined template.
- **Listener** – Listens to messages from **RabbitMQ** and triggers appropriate backend logic.

### Communication Between Microservices

We’ll explore multiple strategies for inter-service communication:

- **REST API** with JSON as transport
- **RPC** (Remote Procedure Call)
- **gRPC** using Protocol Buffers for high performance
- **AMQP** (Advanced Message Queuing Protocol) for event-driven messaging with RabbitMQ

---

## 📁 Project Structure

Each folder corresponds to a specific lesson/module:

- `01 - Introduction`
- `02 - Building a Simple Front End and One Microservice`
- `03 - Building an Authentication Service`
- `04 - Building a Logger Service`
- `05 - Building a Mail Service`
- `06 - Building a Listener Service AMQP with RabbitMQ`
- `07 - Communicating Between Services using Remote Procedure Calls (RPC)`
- `08 - Speeding Things Up (Potentially) with gRPC`
- `09 - Deploying Our Distributed App using Docker Swarm`
- `10 - Deploying Our Distributed App to Kubernetes`
- `11 - Testing Microservices`
- `12 - Final Thoughts`

---

## 📄 Prerequisites

- Go 1.20+
- Docker & Docker Compose
- Kubernetes CLI (`kubectl`)
- RabbitMQ
- PostgreSQL & MongoDB
- gRPC tools
- Make (optional)

---

## 🚀 How to Run

Each module is self-contained. To run a module:

```bash
cd "03 - Building an Authentication Service"
go run
