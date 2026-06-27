# Welcome to the Agapornis Project

**Agapornis** is an open-source ecosystem for managing distributed game servers and containerized applications.

Built around strict mutual TLS (mTLS) and gRPC, it provides a highly secure, modern alternative for developers and sysadmins who want a tightly coupled Node.js control plane and a highly performant .NET native worker daemon.

### Ecosystem

The project is split into two core repositories to maximize developer ergonomics on the frontend and raw machine-code performance on the backend:

**Agapornis Frontend (WOKRING ON)**
The official frontend interface for the Master API. Built with Next.js (React). Because the Master is a pure API, you can use this official panel or easily build your own custom frontend to manage your network.

**Agapornis Master (WORKING ON)**
The central control plane and web panel. Built with **NestJS (TypeScript)**. It acts as the internal Certificate Authority (CA), orchestrates worker nodes, manages the UI, and issues mTLS certificates.

* **Agapornis Agent (BETA)**
The remote worker daemon. Built with **C# (.NET 10 Native AOT)**. It runs on your worker nodes, communicates exclusively over mTLS, and manages the actual Docker containers and system resources with millisecond startup times.

###  Community & Status

> **Status: Early Alpha**
> The Agapornis ecosystem is currently undergoing active development. We are building this in the open to share our architecture and learn from the community.

Contributions, security audits, bug reports, and architectural discussions are highly encouraged! Feel free to open an issue or submit a pull request if you want to help out.
