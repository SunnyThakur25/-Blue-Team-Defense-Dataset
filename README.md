# -Blue-Team-Defense-Dataset
A structured, multi-format collection of detection rules mapped to real-world threats. This dataset is designed for blue teamers, threat detection engineers, SOC analysts, and cybersecurity researchers who work on detecting adversarial activity through rule-based systems such as Sigma, YARA, and Suricata.
# Blue Team Defense Dataset

A structured, multi-format collection of detection rules mapped to real-world threats. This dataset is designed for blue teamers, threat detection engineers, SOC analysts, and cybersecurity researchers who work on detecting adversarial activity through rule-based systems such as Sigma, YARA, and Suricata.

---

## 📁 Dataset Overview

Each entry in this dataset represents a rule designed to detect specific threat behaviors. Rules are structured with MITRE ATT&CK technique mappings and threat types, and are categorized by detection format (Sigma, YARA, Suricata, etc.).

---

## 🔍 Fields

| Field              | Description |
|--------------------|-------------|
| `id`               | Unique identifier for the rule |
| `threat`           | Description of the malicious behavior being detected |
| `rule_type`        | Type of rule (e.g., `Sigma`, `YARA`, `Suricata`) |
| `signature`        | The rule logic or detection pattern |
| `tool`             | The detection platform/tool for which the rule was written |
| `mapped_technique` | Mapped MITRE ATT&CK technique ID (e.g., `T1059.001`) |

---

## 🧪 Example Entries

```json
{
  "id": "01",
  "threat": "PowerShell Abuse",
  "rule_type": "Sigma",
  "signature": "selection: CommandLine contains 'Invoke-Expression'",
  "tool": "Sigma",
  "mapped_technique": "T1059.001"
}
✅ Use Cases

    Building detection engines for SOC environments

    Fine-tuning LLMs for threat hunting or alert generation

    Developing simulation tools and threat modeling assistants

    Educating cybersecurity professionals on detection engineering

🎯 Detection Types Covered

    PowerShell abuse

    Credential dumping

    Ransomware behavior

    Malicious downloads

    Phishing via script execution

🧠 Mapped Framework

    MITRE ATT&CK techniques are used for each detection

    Includes diverse tactics: Execution, Credential Access, Impact, Initial Access

🛡 Tools Represented

    Sigma (SIEM-focused detection)

    YARA (file/memory scanning)

    Suricata (network-based intrusion detection)

📜 License

This dataset is provided under the MIT License. You are free to use, modify, and distribute with attribution.
📫 Contributions

Want to contribute detection rules or expand coverage? Pull requests and community enhancements are welcome!
