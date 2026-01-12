# Getting Started with ConfigCobra

Follow these simple steps to set up ConfigCobra and run your first CIS compliance assessment for Microsoft 365.

Learn more at [configcobra.com](https://configcobra.com)

> ⚠️ **Important License Requirements**
> 
> CIS Benchmarks are based on **Microsoft 365 E3 and E5 licenses**. Although we can scan some controls without them, having some kind of **Microsoft Defender license** (Defender for Office 365, Defender for Endpoint, or Microsoft Defender XDR) is a **minimum requirement** for full functionality.

## Step-by-Step Setup Guide

### Step 1: Get started on Microsoft AppSource

Visit the [Microsoft AppSource marketplace](https://marketplace.microsoft.com/en-us/product/saas/nologiesholdingkorltoltfelelssgtrsasg1726131505636.config_cobra_01?tab=Overview) to acquire your ConfigCobra subscription.

1. Go to Microsoft AppSource and press **"Get it now"**

   ![Get it now button on Microsoft AppSource](../images/MicrosoftAppSource/01_GetItNow.png)

2. To acquire a free trial, please select the **Standard** plan

   ![Select Standard plan for free trial](../images/MicrosoftAppSource/02_Plan.png)

### Step 2: Provide your user count

Enter the number of licensed users in your organization. **This is important** because the application only works if you have that many licenses as many licensed users you have (excluded guest users).

![Terms and user count selection](../images/MicrosoftAppSource/03_Terms&UserCount.png)

### Step 3: Complete your order

Select your billing account and billing profile, then place your order through the Microsoft AppSource checkout process.

![Select billing account](../images/MicrosoftAppSource/04_BillingAccount.png)

![Complete purchase](../images/MicrosoftAppSource/05_CompletePurchase.png)

### Step 4: Activate your subscription

Follow the activation link to our fulfillment platform and activate your subscription. This link will be provided after you complete your purchase on Microsoft AppSource.

![Activate subscription](../images/MicrosoftAppSource/06_ActivateSubscription.png)

### Step 5: Receive confirmation email

Once your subscription is activated by our team, you will receive a confirmation email with your login credentials and next steps.

![Activation confirmation email](../images/MicrosoftAppSource/07_ActivationEmail.png)

### Step 6: Log in to ConfigCobra

Head to [app.configcobra.com](https://app.configcobra.com) and log in using the credentials from your confirmation email.

### Step 7: Accept permissions

Accept all the permissions on the admin consent page. This is required for ConfigCobra to access and assess your Microsoft 365 configurations.

![Admin consent page - Part 1](../images/MicrosoftAppSource/08_AdminConsent1.png)

![Admin consent page - Part 2](../images/MicrosoftAppSource/09_AdminConsent2.png)

### Step 8: Configure missing permissions

After login, go to the **Assessment page**. You will see some controls that have a **Role required** blue tag.

![Assessment page with Role required tags](../images/MicrosoftAppSource/10_RolePermissions.png)

**If you are an administrator:**
- Select all permissions as an administrator and activate them

**If you are a regular user:**
- Send the instructions provided in the **Do It Manually** section to your global administrator to grant the necessary permissions

  ![Assign role permissions as administrator](../images/MicrosoftAppSource/11_RolePermissionsAssign.png)



## You're Ready!

Once you've completed all the steps above, you can navigate to the Assessment page and start running your first CIS compliance scan. ConfigCobra will automatically check your Microsoft 365 configurations against CIS Benchmark standards.

Visit [configcobra.com](https://configcobra.com) for additional resources and support.

## Next Steps

- Learn how to [run assessments](./assessments.md)
- Understand [assessment results](./reports.md)
- Create [custom rule sets](./rule-sets.md)
- Set up [scheduled scans](./schedules.md)

---

[← Back to Documentation](../README.md) | [Next: Assessments →](./assessments.md)

