# PCI-DSS-v4.0-Compliance-Assessment

This initiative covers a complete compliance and security assessment for an e-commerce platform under PCI DSS v4.0 (SAQ D / ROC), cross-mapped with ISO/IEC 27001:2022 Annex A controls:  Scoping & Data Flow Mapping: Traced cardholder data paths across client apps, Node.js payment APIs, AWS infrastructure, and MySQL databases to define the Cardholder Data Environment (CDE) boundaries.

Technical Security Audit: Identified critical vulnerabilities across PCI DSS v4.0 domains—notably plain-text CVV storage in temporary disk files (/tmp/pending_cvv.txt), card data exposure in production debug logs (/var/log/app/debug.log), and missing EDR/SAST controls.

Dual-Framework Mapping: Aligned technical vulnerabilities directly with ISO/IEC 27001:2022 Annex A controls (e.g., Data Leakage Prevention, Secure Development, Logging, and Malware Protection). 

3-Phase Remediation Roadmap: Formulated a prioritized strategy covering immediate containment (purging SAD disk storage and masking logs), strategic technical integration (deploying EDR, adding SAST to CI/CD, and replacing shared SSH keys with MFA), and final audit validation (VPC micro-segmentation, quarterly ASV scans, and ROC sign-off).
