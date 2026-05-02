# Assignment-4 Computer Networks

## Submitted By
- **Name:** Srshti Jain  
- **Roll Number:** 2301730107 
- **Program:** B.Tech CSE (AI/ML)  
- **Section:** B  
- **Course:** Computer Networks Lab  
- **Course Code:** ENCS304  

---

# Overview

This assignment demonstrates the configuration of a **DNS Server** using **Cisco Packet Tracer** and explains how domain names are translated into IP addresses within a local network.

---

# Network Design

## Devices Used

- 1 Server (DNS Server)  
- 2–3 PCs  
- 1 Switch  

## Topology

PCs → Switch → Server

---

# IP Configuration

## Server Configuration

| Device | IP Address | Subnet Mask |
|--------|------------|-------------|
| Server | 192.168.1.2 | 255.255.255.0 |

## PC Configuration

| Device | IP Address | Subnet Mask | DNS Server |
|--------|------------|-------------|------------|
| PC1 | 192.168.1.3 | 255.255.255.0 | 192.168.1.2 |
| PC2 | 192.168.1.4 | 255.255.255.0 | 192.168.1.2 |
| PC3 | 192.168.1.5 | 255.255.255.0 | 192.168.1.2 |

---

# DNS Configuration

The following DNS records were added:

| Domain Name | IP Address |
|------------|------------|
| www.example.com | 192.168.1.2 |
| www.google.com | 192.168.1.2 |

---

# Testing Commands

## Ping Test

```bash
ping www.example.com
ping www.google.com
```
## NSLOOKUP Test
```bash
nslookup www.example.com
nslookup www.google.com
```
## Traceroute Test
```bash
tracert www.example.com
```

---

# Analysis

## 1. Query Time

- Approximate response time: **1–2 ms**
- Low latency because all devices are connected in the same local network.

## 2. Response Accuracy

- Domain names were resolved correctly to the assigned IP address.

## 3. Name Resolution Process

1. User enters a domain name in the browser or command prompt.  
2. Request is sent to the configured DNS server.  
3. DNS server checks records and returns the mapped IP address.  
4. Communication is established with the destination host.  

---

# Key Observations

- DNS converts easy-to-remember domain names into IP addresses.  
- Correct IP and DNS configuration is necessary for successful communication.  
- DNS resolution and physical network connectivity are separate processes.  
- Cisco Packet Tracer simulates DNS locally and does not provide real internet access.  

---

# Conclusion

The DNS server was successfully configured and tested in Cisco Packet Tracer.  

The system accurately resolved domain names with minimal delay, demonstrating efficient DNS functionality in a local area network.

---

# Tools Used

- Cisco Packet Tracer  
- Command Prompt  
