# Changelog

All notable changes to ConfigCobra will be documented in this file.

The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).

## [1.0.0] - 2024-11-01

### 🎉 Initial Release

We're excited to announce the first release of ConfigCobra v1.0.0 - your comprehensive solution for automated CIS compliance assessment for Microsoft 365 environments.

### ✨ Added

#### Core Features
- ✅ **Automated CIS Compliance Assessments** - Complete automated assessment of all 129 CIS controls for Microsoft 365 Foundations Benchmark
- ✅ **Level 1 & Level 2 Benchmarks** - Support for both essential and enhanced security controls
- ✅ **Real-time Configuration Detection** - Detects configuration drift in real-time
- ✅ **Fast Assessment Times** - Typical scan duration of 20-25 minutes (depending on user count)

#### Assessment Capabilities
- ✅ **Ad-Hoc (Manual) Assessments** - Run assessments on-demand at any time
- ✅ **Flexible Benchmark Selection** - Choose specific benchmarks, rule sets, or comprehensive coverage
- ✅ **Assessment Overview** - Preview scan configuration and controls to be assessed
- ✅ **Assessment History** - View last assessment results on the Assessment page

#### Scheduled Assessments
- ✅ **Flexible Scheduling** - Daily, weekly, monthly, or custom schedules
- ✅ **Rule Set Integration** - Use custom rule sets or specific benchmark selections in schedules
- ✅ **Multiple Schedules** - Create and manage multiple schedules for different compliance needs
- ✅ **Automated Execution** - Assessments run automatically at scheduled times

#### Custom Rule Sets
- ✅ **Create Custom Collections** - Build personalized sets of CIS controls tailored to your organization
- ✅ **Descriptive Naming** - Add names and descriptions to identify rule set purposes
- ✅ **Easy Management** - Edit or delete rule sets as your needs evolve
- ✅ **Seamless Integration** - Use rule sets in both manual and scheduled assessments

#### CIS-Approved Reports
- ✅ **Audit-Ready PDFs** - Download CIS-approved and certified PDF reports for audit submission
- ✅ **Summary Tab** - High-level overview with compliance scores and key findings
- ✅ **Details Tab** - Results organized by benchmark with individual control details
- ✅ **Historical Tracking** - View and compare assessment results over time
- ✅ **Tenant Configuration View** - See current settings in your tenant for each control

#### Assessment Outcomes
- ✅ **Pass Status** - Control fully complies with CIS Benchmark requirements
- ✅ **Fail Status** - Control does not meet CIS Benchmark requirements
- ✅ **Partial Pass Status** - Control partially meets requirements

#### Detailed Control Information
- ✅ **Outcome Status** - Pass, Fail, or Partial Pass
- ✅ **Description** - Detailed explanation of the control
- ✅ **Impact** - Security and compliance implications
- ✅ **Audit** - Evidence and audit trail information
- ✅ **Remediation** - Step-by-step instructions to fix issues
- ✅ **Configuration** - Current settings in your tenant

#### Multi-Standard Compliance Mapping (Theoretical)
- ✅ **24+ Security Standards** - Comprehensive theoretical mapping between CIS Microsoft 365 controls and multiple compliance frameworks including:
  - SOC 2
  - NIS2
  - HIPAA
  - PCI DSS
  - ISO 27001
  - ISO/IEC 27002:2022
  - NIST CSF
  - NIST SP 800-53 R5
  - CMMC
  - And 14+ more standards

**Note:** Framework-specific certified reports are planned for future releases. Currently, only CIS-certified reports are available. The mapping data is theoretical and can be used alongside CIS reports to understand compliance relationships.

#### User Management & Access Control
- ✅ **Azure Entra Integration** - Seamless integration with Azure Entra (formerly Azure Active Directory)
- ✅ **Single Sign-On (SSO)** - Users authenticate using existing Azure Entra credentials
- ✅ **Tenant Security** - Only users from your subscribed tenant can be added
- ✅ **Role-Based Access Control** - Three distinct role levels:
  - **Global Admin** - Full administrative access
  - **Global Operator** - Operational access to run assessments
  - **Global Reader** - Read-only access

#### Notifications
- ✅ **Windows Notifications** - Real-time desktop notifications for ad hoc scan completion
- ✅ **Email Notifications** - Comprehensive email updates for:
  - Assessment runs (scheduled and manual)
  - User changes (added, deleted, or edited)
  - Permission changes
  - Important account events

#### Settings & Customization
- ✅ **Custom Color Themes** - Personalize your ConfigCobra interface
- ✅ **Notification Preferences** - Configure Windows and email notification settings
- ✅ **Account Settings** - Manage account preferences

#### Microsoft AppSource Integration
- ✅ **Marketplace Availability** - Available through Microsoft AppSource marketplace
- ✅ **Free Trial** - Standard plan available with free trial option
- ✅ **User-Based Licensing** - Licensing based on number of licensed users
- ✅ **Fulfillment Platform** - Seamless subscription activation

### 📚 Documentation

- ✅ Complete user documentation
- ✅ Getting Started guide
- ✅ Feature-specific guides (Assessments, Reports, Rule Sets, Schedules, etc.)
- ✅ Screenshots and visual guides
- ✅ Example reports

### 🔗 Links & Resources

- ✅ Application: [app.configcobra.com](https://app.configcobra.com)
- ✅ Website: [configcobra.com](https://configcobra.com)
- ✅ Microsoft AppSource: Available for subscription
- ✅ GitHub: Documentation and issue tracking

---

## Release Notes Format

Each release will follow this structure:
- **Version Number** - [Semantic Versioning](https://semver.org/)
- **Release Date** - YYYY-MM-DD format
- **Added** - New features
- **Changed** - Changes to existing functionality
- **Deprecated** - Soon-to-be removed features
- **Removed** - Removed features
- **Fixed** - Bug fixes
- **Security** - Security updates

---

**ConfigCobra** - Automated CIS Compliance for Microsoft 365 | [configcobra.com](https://configcobra.com)

