# Secure Shell (SSH) Study Notes - [Link to article](https://www.cloudflare.com/learning/access-management/what-is-ssh/)

## What is SSH?
Secure Shell (SSH) is a protocol used to securely send commands and data over an unsecured network. It uses cryptography to authenticate and encrypt connections between devices, allowing for remote management, secure file transfers, and tunneling (port forwarding).

## Key Features of SSH
- **Remote Encrypted Connections**: SSH establishes a secure connection between a user's device and a remote machine, using encryption to protect data from interception.
- **Tunneling (Port Forwarding)**: SSH enables data packets to traverse networks they otherwise couldn't by encapsulating them in headers that alter their destination.

## How SSH Works
1. **Runs on TCP/IP**: SSH operates over the TCP/IP suite, which routes and delivers packets across networks.
2. **Public Key Cryptography**: Uses asymmetric encryption with public/private key pairs for authentication and secure communication.
3. **Authentication**: Requires user authentication (e.g., username/password) to ensure secure access.

## SSH Tunneling (Port Forwarding)
Port forwarding allows data to be securely sent from one machine to another. This is useful for accessing private networks remotely and bypassing firewall restrictions.

## Using SSH
- Linux and macOS have built-in SSH clients (accessible via Terminal).
- Windows may require an external SSH client.
- Common use cases:
  - Remote server and infrastructure management
  - Secure file transfers (more secure than FTP)
  - Remote access to cloud services and private networks
  - Firewall bypassing

## SSH Port
- **Default port**: 22
- Firewalls often leave port 22 open, allowing SSH traffic to pass through.

## Security Risks
- **SSH Key Theft**: Attackers can steal SSH keys to gain unauthorized access.
- **Persistent Access**: Poor SSH key management can lead to long-term security breaches.
- **Backdoors & Data Extraction**: SSH tunnels can be exploited to move sensitive data.

## SSH vs. Other Tunneling Protocols
- **IPsec, GRE, IP-in-IP**: Operate at the network layer and encrypt all traffic.
- **SSH**: Operates at the application layer, encrypting only specific applications.
- **TCP vs. UDP**: SSH uses TCP for reliable data transfer, whereas IPsec often uses UDP for speed but with potential packet loss.