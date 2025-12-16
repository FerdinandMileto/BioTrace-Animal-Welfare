🐾 BIOTRACE Protocol: The Immutable Life Ledger

[![Solidity](https://img.shields.io/badge/Solidity-0.8.20-363636?style=for-the-badge&logo=solidity&logoColor=white)](https://soliditylang.org/)
[![IPFS](https://img.shields.io/badge/Storage-IPFS-65C2CB?style=for-the-badge&logo=ipfs&logoColor=white)](https://ipfs.tech/)
[![Impact](https://img.shields.io/badge/Focus-Social_Impact-ff0055?style=for-the-badge)](https://santuarioixtlan.com)
[![Status](https://img.shields.io/badge/Status-Deployed_Alpha-success?style=for-the-badge)]()

> **"Paper records fade and burn. The Blockchain remembers forever."**



---

## 🧬 Abstracto Ejecutivo

**BioTrace** no es una colección de NFTs. Es una infraestructura de **Identidad Soberana para el Bienestar Animal**.

Durante **10 años**, he dirigido operaciones de rescate en el **Santuario Ixtlán**, enfrentando dos problemas sistémicos: la opacidad en el uso de donaciones y la pérdida crítica de historiales médicos en adopciones.

Como Ingeniero en Sistemas y Data Scientist, decidí que la solución no era burocracia, sino criptografía. **BioTrace convierte la vida de un ser vivo rescatado en un activo digital inmutable**, garantizando trazabilidad absoluta desde el rescate hasta la adopción.

---

## ⚙️ Arquitectura del Sistema

El protocolo opera bajo un estándar modificado de **ERC-721 (NFTs dinámicos)**, funcionando como el expediente médico y legal del animal.

### 🔄 El Ciclo de Vida "On-Chain"

1.  **Génesis (Rescue Mint):**
    *   Al rescatar a un animal, se acuña un Token Único.
    *   Estado inicial: `Status: Critical`. La metadata se ancla en IPFS (resistente a censura).
    
2.  **Trazabilidad Médica (Immutable Logs):**
    *   Cada vacuna, cirugía o tratamiento se registra mediante la función `addMedicalRecord`.
    *   A diferencia de una base de datos SQL que puede ser alterada, **nadie puede borrar una vacuna de la Blockchain**. Esto da certeza matemática a los adoptantes.

3.  **Transparencia de Recursos (Smart Donations):**
    *   Los donadores pueden ver el TxHash (Hash de Transacción) de cada intervención médica. "Tu dinero no se perdió; se convirtió en el bloque #482910 que pagó esta cirugía".

4.  **Adopción (Ownership Transfer):**
    *   Al adoptar, el NFT (y la responsabilidad legal) se transfiere a la Wallet del nuevo dueño. El historial viaja con él, indestructible.

---

## 🛠️ Stack Tecnológico

Este proyecto demuestra la implementación de patrones de diseño de software avanzados aplicados a problemas del mundo real:

*   **Smart Contracts:** Solidity `^0.8.20` (OpenZeppelin Secured).
*   **Storage:** IPFS (InterPlanetary File System) para persistencia de imágenes y JSON.
*   **Data Structures:** `Structs` complejos y `Mappings` para gestión eficiente de expedientes.
*   **Events:** Sistema de emisión de eventos para indexación en Dashboards Frontend.

```solidity
// Core Logic Snippet
struct MedicalRecord {
    string date;
    string treatment;
    string vetLicense; // Trazabilidad profesional
}
mapping(uint256 => MedicalRecord[]) public medicalHistory;
🌍 Visión & Scalability
Actualmente desplegado en Testnet (Remix VM) para el Santuario Ixtlán.
La visión es escalar BioTrace como un Protocolo de Código Abierto (Open Source) para cualquier ONG en Latinoamérica que desee transparentar sus operaciones y modernizar sus adopciones.
"No usamos tecnología por moda. La usamos para dar voz y memoria a quienes no la tienen."

👨‍💻 Developed by
Fernando Gutiérrez Berumen
Full-Stack Engineer | Web3 Strategist | Director @ Santuario de animales Ixtlán 
