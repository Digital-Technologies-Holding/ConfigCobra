# Compliance Standard Mapping

ConfigCobra provides comprehensive **theoretical mapping** between CIS Microsoft 365 Foundations Benchmark controls and various security and compliance frameworks. This mapping helps you understand how CIS assessments relate to other compliance standards.

**⚠️ Important:** ConfigCobra currently generates **CIS-certified reports only**. Framework-specific certified reports (e.g., SOC 2-certified, HIPAA-certified) are planned for future releases. The mapping data provided here is theoretical and can be used alongside CIS reports to support compliance with other standards.

This document details the coverage and mapping statistics for each supported standard.

## 📊 Mapping Overview

The following table shows how CIS Microsoft 365 Foundations Benchmark controls map to various compliance frameworks and directives:

| Directive | All Directive Controls | Mapped to CIS M365 | Mapped to CIS M365 (%) | All CIS M365 Controls | CIS M365 Mapped to Directive | CIS M365 Mapped to Directive (%) |
|-----------|----------------------|-------------------|----------------------|---------------------|----------------------------|--------------------------------|
| HIPAA | 75 | 32 | 42.67% | 141 | 51 | 36.17% |
| ISO/IEC 27001:2022 | 232 | 29 | 12.50% | 141 | 100 | 70.92% |
| MCSB | 169 | 27 | 15.98% | 141 | 83 | 58.87% |
| NIS2 | 159 | 28 | 17.61% | 141 | 76 | 53.90% |
| PCI DSS | 385 | 64 | 16.62% | 141 | 94 | 66.67% |
| CMMC | 236 | 38 | 16.10% | 141 | 89 | 63.12% |
| CPGs | 161 | 9 | 5.59% | 141 | 45 | 31.91% |
| CRI | 331 | 22 | 6.65% | 141 | 65 | 46.10% |
| CSA CCM v4 | 250 | 32 | 12.80% | 141 | 71 | 50.35% |
| Cyber Essentials v2.2.2 | 180 | 24 | 13.33% | 141 | 84 | 59.57% |
| FFIEC CAT 2 | 181 | 29 | 16.02% | 141 | 83 | 58.87% |
| GSMA FS.31 | 58 | 14 | 24.14% | 141 | 71 | 50.35% |
| ISACA | 89 | 4 | 4.49% | 141 | 41 | 29.08% |
| ISO/IEC 27002:2022 | 243 | 30 | 12.35% | 141 | 102 | 72.34% |
| NCSC | 83 | 12 | 14.46% | 141 | 58 | 41.13% |
| NERC | 117 | 21 | 17.95% | 141 | 79 | 56.03% |
| NIST CSF | 211 | 21 | 9.95% | 141 | 90 | 63.83% |
| NIST CSF 2.0 | 112 | 9 | 8.04% | 141 | 37 | 26.24% |
| NIST SP 800-171 R2 | 138 | 24 | 17.39% | 141 | 70 | 49.65% |
| NIST SP 800-53 R5 | 345 | 55 | 15.94% | 141 | 108 | 76.60% |
| NYDFS | 151 | 18 | 11.92% | 141 | 54 | 38.30% |
| NZISM | 1,420 | 66 | 4.65% | 141 | 97 | 68.79% |
| SOC 2 | 155 | 10 | 6.45% | 141 | 86 | 60.99% |
| TSA | 73 | 9 | 12.33% | 141 | 64 | 45.39% |

## 📈 Understanding the Mapping

### Column Descriptions

- **All Directive Controls** - Total number of controls in the compliance framework
- **Mapped to CIS M365** - Number of framework controls that map to CIS M365 controls
- **Mapped to CIS M365 (%)** - Percentage of framework controls covered by CIS M365
- **All CIS M365 Controls** - Total CIS Microsoft 365 Foundations Benchmark controls (141)
- **CIS M365 Mapped to Directive** - Number of CIS M365 controls that map to the framework
- **CIS M365 Mapped to Directive (%)** - Percentage of CIS M365 controls that map to the framework

### What This Means

**High "CIS M365 Mapped to Directive (%)"** indicates:
- ✅ Strong alignment between CIS M365 and the framework
- ✅ Most CIS controls are relevant to the framework
- ✅ Comprehensive coverage when running CIS assessments

**High "Mapped to CIS M365 (%)"** indicates:
- ✅ Many framework controls are covered by CIS M365
- ✅ Running CIS assessments addresses significant portion of framework requirements
- ✅ Fewer additional controls may be needed

## 🎯 Standards by Coverage Category

### Excellent Coverage (70%+ CIS M365 Mapped)
- ✅ **ISO/IEC 27002:2022** - 72.34%
- ✅ **NIST SP 800-53 R5** - 76.60%
- ✅ **ISO/IEC 27001:2022** - 70.92%
- ✅ **NZISM** - 68.79%

### Good Coverage (60-70% CIS M365 Mapped)
- ✅ **PCI DSS** - 66.67%
- ✅ **NIST CSF** - 63.83%
- ✅ **CMMC** - 63.12%
- ✅ **SOC 2** - 60.99%
- ✅ **Cyber Essentials v2.2.2** - 59.57%

### Moderate Coverage (40-60% CIS M365 Mapped)
- ✅ **NERC** - 56.03%
- ✅ **NIS2** - 53.90%
- ✅ **CSA CCM v4** - 50.35%
- ✅ **GSMA FS.31** - 50.35%
- ✅ **NIST SP 800-171 R2** - 49.65%
- ✅ **CRI** - 46.10%
- ✅ **TSA** - 45.39%
- ✅ **HIPAA** - 36.17%

## 💡 How to Use This Mapping

**Important Reminder:** ConfigCobra currently generates **CIS-certified reports only**. This mapping is theoretical and helps you understand relationships between CIS controls and other frameworks. Framework-specific certified reports are planned for future releases.

### 1. Assessment Planning
- Identify which standards apply to your organization
- Review coverage percentages to understand how CIS assessments relate to your compliance needs
- Create rule sets focused on CIS controls that map to your compliance requirements

### 2. Gap Analysis
- Understand which framework controls are not covered by CIS M365
- Plan additional assessments or controls for gaps
- Use mapping to prioritize security improvements within CIS framework

### 3. Audit Preparation
- Use CIS-certified reports along with this mapping documentation
- Demonstrate how CIS assessments support compliance with other standards
- Show comprehensive coverage through CIS assessments with mapping context

### 4. Multi-Standard Compliance Support
- Leverage mapping to show how CIS assessments relate to multiple standards
- Use CIS reports as supporting evidence (with mapping documentation) for various compliance needs
- Understand overlap between standards through mapping data

**Note:** For audit purposes, always clarify that you are using CIS-certified reports with theoretical mapping data. Framework-specific certified reports are not yet available.

## 📋 Framework Descriptions

### Healthcare & Privacy
- **HIPAA** - Health Insurance Portability and Accountability Act
- **NYDFS** - New York Department of Financial Services Cybersecurity Regulation

### International Standards
- **ISO/IEC 27001:2022** - Information Security Management System
- **ISO/IEC 27002:2022** - Information Security Controls
- **NIS2** - EU Network and Information Systems Directive 2

### Government & Defense
- **CMMC** - Cybersecurity Maturity Model Certification
- **NIST SP 800-53 R5** - Security and Privacy Controls
- **NIST SP 800-171 R2** - Protecting Controlled Unclassified Information
- **NIST CSF / NIST CSF 2.0** - Cybersecurity Framework

### Financial Services
- **PCI DSS** - Payment Card Industry Data Security Standard
- **SOC 2** - Service Organization Control 2
- **FFIEC CAT 2** - Federal Financial Institutions Examination Council Cybersecurity Assessment Tool

### Industry-Specific
- **NERC** - North American Electric Reliability Corporation
- **GSMA FS.31** - GSMA Financial Services
- **MCSB** - Microsoft Cloud Security Benchmark
- **NZISM** - New Zealand Information Security Manual

### Regional & National
- **Cyber Essentials v2.2.2** - UK Cyber Essentials
- **NCSC** - National Cyber Security Centre (UK)
- **TSA** - Transportation Security Administration

## 🔍 Best Practices

1. **Start with CIS** - Run comprehensive CIS assessments first (ConfigCobra generates CIS-certified reports only)
2. **Map to Standards** - Use theoretical mapping to understand how CIS controls relate to your frameworks
3. **Create Rule Sets** - Build rule sets focusing on CIS controls that map to your compliance requirements
4. **Regular Assessments** - Schedule CIS assessments based on compliance needs
5. **Document Gaps** - Identify and document controls not covered by CIS M365
6. **Use Mapping Strategically** - Combine CIS-certified reports with mapping documentation to support multi-standard compliance claims

## 📚 Additional Resources

- [CIS Microsoft 365 Foundations Benchmark](https://www.cisecurity.org/benchmark/microsoft_365)
- [ConfigCobra Documentation](./README.md)
- [Use Cases](../use-cases/)

---

**Note**: Compliance mapping is a guide. Always consult with compliance experts and framework documentation for complete requirements.

**Learn More**: Visit [configcobra.com](https://configcobra.com) or contact **info@digitechold.com**

