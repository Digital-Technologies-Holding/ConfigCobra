# Required Permissions

This document describes all required permissions and role assignments for ConfigCobra to function properly.

## Overview

ConfigCobra requires Microsoft Graph API permissions, Office 365 Exchange Online permissions, SharePoint permissions, and Power BI Service permissions to assess your Microsoft 365 environment against CIS security controls. Additionally, certain Azure AD role assignments are recommended for full functionality.

---

## Microsoft Graph Permissions (18 required)

All Microsoft Graph permissions are **Application** permissions (except where noted), which means they are granted to the application itself, not to individual users.

### Required Permissions

#### AccessReview.Read.All
- **Type:** Application
- **Description:** Read all access reviews
- **Required:** Yes
- **Purpose:** Allows ConfigCobra to read access review data for compliance assessment

#### AuditLog.Read.All
- **Type:** Application
- **Description:** Read all audit log data
- **Required:** Yes
- **Purpose:** Essential for reading audit logs to verify compliance with logging requirements

#### DeviceManagementConfiguration.Read.All
- **Type:** Application
- **Description:** Read Microsoft Intune device configuration and policies
- **Required:** Yes
- **Purpose:** Assesses Intune device configuration policies for compliance

#### DeviceManagementServiceConfig.Read.All
- **Type:** Application
- **Description:** Read Microsoft Intune configuration
- **Required:** Yes
- **Purpose:** Reads Intune service configuration settings

#### Directory.Read.All
- **Type:** Application
- **Description:** Read directory data
- **Required:** Yes
- **Purpose:** Reads Azure AD directory information, including users, groups, and organizational data

#### Domain.Read.All
- **Type:** Application
- **Description:** Read domains
- **Required:** Yes
- **Purpose:** Reads domain configuration and domain-related settings

#### Group.Read.All
- **Type:** Application
- **Description:** Read all groups
- **Required:** Yes
- **Purpose:** Reads all groups in the directory for compliance assessment

#### Group.ReadWrite.All
- **Type:** Delegated
- **Description:** Read and write all groups
- **Required:** Yes
- **Purpose:** Allows reading and writing group data (note: ConfigCobra only reads data)

#### GroupMember.Read.All
- **Type:** Delegated
- **Description:** Read group memberships
- **Required:** Yes
- **Purpose:** Reads group membership information for security group assessments

#### Organization.Read.All
- **Type:** Application
- **Description:** Read organization information
- **Required:** Yes
- **Purpose:** Reads organizational information and tenant details

#### OrgSettings-AppsAndServices.Read.All
- **Type:** Application
- **Description:** Read organization-wide apps and services settings
- **Required:** Yes
- **Purpose:** Reads organization-wide application and service settings

#### OrgSettings-Forms.Read.All
- **Type:** Application
- **Description:** Read organization-wide Microsoft Forms settings
- **Required:** Yes
- **Purpose:** Reads Microsoft Forms organization-wide settings

#### Policy.Read.All
- **Type:** Application
- **Description:** Read your organization's policies
- **Required:** Yes
- **Purpose:** Reads organizational policies for compliance assessment

#### RoleManagement.ReadWrite.Directory
- **Type:** Delegated
- **Description:** Read and write directory RBAC settings
- **Required:** Yes
- **Purpose:** Reads and writes role-based access control (RBAC) settings (note: ConfigCobra only reads data)

#### RoleManagementPolicy.Read.Directory
- **Type:** Application
- **Description:** Read all policies for privileged role assignments of your company's directory
- **Required:** Yes
- **Purpose:** Reads privileged role assignment policies

#### SharePointTenantSettings.Read.All
- **Type:** Application
- **Description:** Read SharePoint and OneDrive tenant settings
- **Required:** Yes
- **Purpose:** Reads SharePoint and OneDrive tenant-level settings

#### User.Read.All
- **Type:** Application
- **Description:** Read all users' full profiles
- **Required:** Yes
- **Purpose:** Reads user profile information for compliance assessment

#### User.ReadBasic.All
- **Type:** Delegated
- **Description:** Read all users' basic profiles
- **Required:** No (but recommended)
- **Purpose:** Reads basic user profile information

---

## Office 365 Exchange Online Permissions (1 required)

### Exchange.ManageAsApp
- **Type:** Application
- **Description:** Manage Exchange As Application
- **Required:** Yes
- **Purpose:** Allows ConfigCobra to read Exchange Online configuration and settings for compliance assessment

---

## SharePoint Permissions (1 required)

### Sites.FullControl.All
- **Type:** Application
- **Description:** Have full control of all site collections
- **Required:** Yes
- **Purpose:** Reads SharePoint site collection settings and configurations (note: ConfigCobra only reads data, does not modify)

---

## Power BI Service Permissions (1 required)

### Tenant.ReadWrite.All
- **Type:** Delegated
- **Description:** Read and write all content in tenant
- **Required:** Yes
- **Purpose:** Reads Power BI tenant settings for compliance assessment (note: ConfigCobra only reads data)

---

## Azure AD Role Assignments (Recommended)

The following Azure AD roles are **not strictly required** but are recommended for full functionality. Without these roles, some standard assessments may not be possible.

### Required Roles for Full Functionality

#### Global Reader
- **Purpose:** Provides read-only access to most Azure AD objects and settings
- **Impact if missing:** Some standard assessments may not be possible

#### Security Reader
- **Purpose:** Read-only access to security-related information in Microsoft 365
- **Impact if missing:** Security-related assessments may be limited

#### Insights Administrator
- **Purpose:** Access to insights and analytics data
- **Impact if missing:** Some analytics-based assessments may not be available

### Security Group Configuration

A security group named **ConfigCobraAPI** will be created automatically. This group is used for:

- Service principal access management
- Fabric (Power BI) configuration: "Service principals can access read-only admin APIs"
- Setting: **Enabled for a subset of the organization**

---

## Permission Grant Process

1. **Admin Consent Required:** All Application permissions require admin consent from a Global Administrator or Privileged Role Administrator.

2. **Grant Location:** Permissions are granted in the Azure AD App Registration under "API permissions."

3. **Consent Type:** 
   - Application permissions require admin consent for the entire organization
   - Delegated permissions can be consented by individual users or admins

4. **Verification:** After granting permissions, verify that all permissions show "Granted for [Your Organization Name]."

---

## Security Considerations

### Read-Only Operations
ConfigCobra is designed to **read only** - it does not modify any settings in your Microsoft 365 environment. All write permissions (Group.ReadWrite.All, RoleManagement.ReadWrite.Directory, Tenant.ReadWrite.All) are used only for reading data, not for making changes.

### Least Privilege Principle
While ConfigCobra requires broad read permissions to assess your entire environment, it follows the principle of least privilege:
- Only reads data necessary for compliance assessment
- Does not modify any configurations
- Does not access user content (emails, files, etc.)
- Only accesses configuration and settings data

### Data Handling
- All data access complies with Microsoft's security standards
- Data is used solely for compliance assessment purposes
- No data is stored outside of your Microsoft 365 environment (unless explicitly configured)

---

## Troubleshooting

### Common Issues

**Issue:** Application shows "Internal error" when running assessments
- **Possible causes:**
  - Missing required permissions
  - Admin consent not provided for all permissions
  - Role assignments not properly configured
- **Solution:** 
  1. Verify that all required permissions are granted and admin consent has been provided
  2. Check Azure AD App Registration > API permissions to ensure all permissions show "Granted for [Your Organization]"
  3. Ensure the ConfigCobraAPI security group is created and properly configured
  4. Verify role assignments (Global Reader, Security Reader, Insights Administrator) are in place

**Issue:** "Internal error" appears for specific assessment types
- **Possible causes:**
  - Missing specific permission for that assessment type
  - Role assignment missing for that functionality
  - Service principal not properly configured
- **Solution:**
  - For Power BI assessments: Verify Tenant.ReadWrite.All permission is granted and Fabric settings are configured
  - For Exchange assessments: Verify Exchange.ManageAsApp permission is granted
  - For SharePoint assessments: Verify Sites.FullControl.All permission is granted
  - Check that required role assignments are in place

**Issue:** "Internal error" after initial setup
- **Possible causes:**
  - Permissions not fully propagated
  - Security group configuration incomplete
- **Solution:**
  1. Wait 5-10 minutes after granting permissions for propagation
  2. Ensure ConfigCobraAPI security group exists and is properly configured
  3. Verify Fabric settings: "Service principals can access read-only admin APIs" is enabled for a subset of the organization
  4. Try running the assessment again after waiting for propagation

---

## Support

If you encounter issues with permissions or role assignments, please contact support through configcobra.com or refer to the getting-started guide.

---

**Last Updated:** 2026-01-10

