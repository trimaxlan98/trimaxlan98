# Portafolio de Ciberseguridad & Web3 - Alan Rosas
![Cybersecurity](https://img.shields.io/badge/Focus-Cybersecurity%20%26%20Pentesting-red)
![Web3](https://img.shields.io/badge/Tech-Web3%20%26%20Blockchain-blue)
![Status](https://img.shields.io/badge/Status-Open%20to%20Work-green)

**Ingeniero en Telemática | Investigador de Maestría (IPN) | Especialista en Seguridad Ofensiva**

> Este repositorio documenta casos de estudio técnicos, metodologías de auditoría y proyectos de investigación en ciberdefensa.

---

## 🛠 Arsenal Técnico

| Dominio | Herramientas y Tecnologías |
| :--- | :--- |
| **Auditoría & Pentesting** | Metasploit, Burp Suite, Nmap, Wireshark, Kali Linux, SDR |
| **Web3 Security** | Smart Contract Auditing, Post-Quantum Crypto, EVM, Solidity |
| **Infraestructura** | Linux Hardening (RHEL/Debian), Docker, Qubernetes, WAF/Firewalls |
| **Desarrollo** | Python (SecScripts), C/C++, Bash |

---

## 📂 Casos de Estudio Selectos

### 1. Sistema de Ciberdefensa Cognitiva Satelital 🛰️
*(En colaboración con CIDEFAM / Proceso de Patente)*

**El Reto:** Proteger enlaces satelitales críticos contra guerra electrónica y ataques de denegación de servicio en entornos de alta latencia.

**Solución Técnica:**
- Desarrollo de un **Sistema de Defensa Cognitiva** utilizando Python y Machine Learning.
- Análisis de patrones de tráfico en tiempo real para detección de anomalías.
- Implementación de protocolos propietarios para soberanía tecnológica.

**Metodología:** `Traffic Analysis` -> `Anomaly Detection` -> `Automated Mitigation`

---

### 2. Seguridad Web3 y Algoritmos Post-Cuánticos ⛓️
**El Reto:** Auditar la resistencia de sistemas blockchain actuales frente a la amenaza de la computación cuántica.

**Detalles Técnicos:**
- **Auditoría de Smart Contracts:** Revisión de lógica para prevenir ataques de *Reentrancy* y *Front-running*.
- **Criptografía PQC:** Implementación experimental de firmas digitales basadas en retículos (Lattice-based cryptography).
- **Hardening de Nodos:** Aseguramiento de la infraestructura subyacente de la red blockchain.

```solidity
// Ejemplo conceptual: Validación de seguridad en contrato
modifier nonReentrant() {
    require(_status != _ENTERED, "ReentrancyGuard: reentrant call");
    _status = _ENTERED;
    _;
    _status = _NOT_ENTERED;
}
