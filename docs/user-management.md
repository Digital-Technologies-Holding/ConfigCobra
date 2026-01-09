# User Management

Manage team access, assign roles, and control permissions in ConfigCobra using Azure Entra integration.

## Overview

All user management in ConfigCobra is handled with **Azure Entra** (formerly Azure Active Directory). Only users from your **subscribed tenant** can be added to your ConfigCobra team. This ensures secure access control and seamless integration with your existing identity management infrastructure.

**Single Sign-On (SSO):** Users authenticate using their existing Azure Entra credentials, providing a seamless and secure login experience without separate passwords or accounts.

## How to Manage Users

### Step 1: Log in to ConfigCobra

Log in at [app.configcobra.com](https://app.configcobra.com) using your credentials.

### Step 2: Navigate to Team page

Go to the **Team** page in the main navigation menu.

### Step 3: Add a new user

To add a user to your team:

1. In the top right corner, select **"Add User"**
2. Search for the desired user in your Azure Entra directory
3. On the left side, press **"Add"**
4. The button text changes to **"In Team"** and the user is added

**Default role:** New users are automatically assigned the **Global Reader** role by default. You can change this role in the actions menu.

### Step 4: Change user role

To change a user's role:

1. In the **actions menu**, select the **edit icon** for the desired user
2. You can select from: **Global Admin**, **Global Operator**, or **Global Reader**
3. Select the desired role and press **"Save"**

### Step 5: Delete a user

To delete a user from your team:

In the **actions menu**, press the **delete button** for the desired user. The user will be removed from your ConfigCobra team. This action cannot be undone.

### Step 6: Email notifications

After adding, removing, or editing a user, each administrator receives a notification email. The affected user also receives an email notification about the change to their account or role. Learn more about [notifications](./notifications.md) and how to configure your email preferences.

## Understanding User Roles

ConfigCobra provides three role levels to control access and permissions. Choose the appropriate role based on each user's responsibilities and requirements.

### Global Admin 👑

Full administrative access to all ConfigCobra features, settings, and user management capabilities.

**Permissions:**
- Manage all assessments and reports
- Configure system settings
- Add, edit, and delete users
- Manage rule sets and schedules
- Access all tenant data

### Global Operator 🔧

Operational access to run assessments, view reports, and manage configurations. Cannot manage users or system settings.

**Permissions:**
- Run and schedule assessments
- View and download reports
- Create and manage rule sets
- Configure assessment settings
- View dashboard and activity logs

### Global Reader 👁️

Read-only access to view assessments, reports, and dashboard data. Cannot make changes or run assessments.

**Permissions:**
- View assessments and results
- Access reports (read-only)
- View dashboard and metrics
- Browse rule sets and configurations
- Cannot run assessments or make changes

## Best Practices

- **Assign Global Admin role only to trusted administrators** who need full system access
- **Use Global Operator role** for team members who run assessments but don't need user management capabilities
- **Grant Global Reader role** to stakeholders who only need to view reports and metrics
- **Regularly review team membership** and remove users who no longer need access
- **Monitor email notifications** to stay informed about user management changes

## Azure Entra Integration

### Benefits

- **Single Sign-On (SSO)** - Users authenticate with existing Azure Entra credentials
- **Centralized Management** - Manage users through Azure Entra
- **Security** - Only users from your subscribed tenant can access ConfigCobra
- **Seamless Integration** - Works with your existing identity management infrastructure

### Requirements

- Users must be in your Azure Entra directory
- Users must be part of your subscribed tenant
- Appropriate Azure Entra permissions for user management

## Use Cases

### Small Teams
- Assign Global Admin to IT administrators
- Use Global Operator for security team members
- Grant Global Reader to executives for reporting

### Large Organizations
- Multiple Global Admins for different departments
- Global Operators for compliance and security teams
- Global Readers for auditors and stakeholders

### Compliance Requirements
- Separate roles for different compliance needs
- Read-only access for auditors
- Operational access for compliance teams

---

[← Back to Documentation](./README.md)

