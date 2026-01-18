---
title: "ThreatCompute: Leveraging LLMs for Automated Threat Modeling of Cloud-Native Applications"
collection: publications
category: conferences
permalink: /publication/2025-10-20-threatcompute
date: 2025-10-20
venue: 'Proceedings of the 2025 Cloud Computing Security Workshop (CCSW '25)'
paperurl: 'https://doi.org/10.1145/3733812.3765533'
citation: 'Wimbauer, A., Muscariello, L., Samain, J., Steger, L., Glas, K., Helm, M., & Carle, G. (2025). ThreatCompute: Leveraging LLMs for Automated Threat Modeling of Cloud-Native Applications. In Proceedings of the 2025 Cloud Computing Security Workshop (pp. 14-27). Association for Computing Machinery. https://doi.org/10.1145/3733812.3765533'
---
The increasing complexity of cloud-native applications has necessitated advanced methodologies for threat modeling and security analysis. This paper presents ThreatCompute, a novel framework that combines LLMs with attack graphs to automate the generation of threat hypotheses and the quantification of risk in Kubernetes environments. While traditional approaches to attack graph generation require significant manual effort from security experts, ThreatCompute leverages LLMs to extract security insights from system information, reducing reliance on manual intervention while maintaining high accuracy and generating context-specific, system-aware threat insights. The framework utilizes the MITRE ATT&CK Matrix and the Microsoft Threat Matrix for Kubernetes as structured domains of possible attack techniques. Based on LLM-generated threat hypotheses and a quantitative risk metric, ThreatCompute constructs detailed attack graphs that illustrate potential attack paths and assess their associated risks. This enables both qualitative and quantitative evaluations of application security across varying levels of granularity. Through real-world examples of Kubernetes applications, we demonstrate the effectiveness of our approach in identifying and quantifying security risks.
