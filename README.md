# EduCredPH – Blockchain-Based Credential Verification System

## Overview
**EduCredPH** is a blockchain-powered platform designed to combat credential fraud in higher education. It was developed as part of my doctoral dissertation and deployed as a two-part system:  
1. A **user-facing system** for students, registrars, and verifiers to issue and validate academic credentials.  
2. A **network management dashboard** to monitor the Hyperledger Fabric blockchain network, manage Docker containers, and control API key access.

## The Problem
- Academic credentials are often verified manually, which leads to delays and potential fraud.
- Registrars lacked a tamper-proof way to ensure the authenticity of issued documents.
- There was no centralized infrastructure to manage blockchain services or user access securely.

## My Solution
- Built a **modular PHP + MySQL system** that allowed:
  - Students to request credentials
  - Registrars to issue and hash records on-chain
  - Employers and verifiers to validate documents via hash/QR
- Designed a **Node.js + Express.js backend API** to interact with the Hyperledger Fabric network
- Created a **Network Monitoring Dashboard** for:
  - Docker container health (peer/orderer nodes)
  - API key generation and access logging
  - Chaincode status and audit trails

## Key Features
- RESTful APIs for credential issuance and validation  
- Document hash generation using SHA-256  
- Real-time Docker container status panel  
- Role-based access (student, registrar, verifier)  
- QR code verification with public lookup  
- Logging and audit trail per credential request  

## Tools & Stack
- **Frontend/UI**: HTML, CSS, Bootstrap  
- **Backend**: PHP, Node.js, Express.js  
- **Blockchain**: Hyperledger Fabric 2.5 (Docker)  
- **Database**: MySQL  
- **Monitoring**: Bash scripts + Node.js dashboard  
- **API Testing**: Postman  
- **Deployment**: Linux server, Docker

## Impact
- Created a secure, verifiable credential issuance flow  
- Demonstrated proof-of-concept for academic blockchain adoption  
- Reduced turnaround time of verification from days to seconds  
- Enabled decentralized validation without compromising data privacy
