# Managing Rule Sets

Create custom collections of CIS controls tailored to your organization's specific compliance needs.

## What are Rule Sets?

Rule sets are designed to help users track their environment where it matters to them. You can select which controls you want to assess in the rule set and manually select it on each assessment run or select this in a [scheduled scan](./schedules.md). That way you know that you are not missing none of the important benchmarks for you.

**Use case:** Create a rule set for "Critical Security Controls" that includes only the most important CIS controls for your organization. Then use this rule set in your regular assessments or scheduled scans to ensure you always check these critical controls.

## How to Manage Rule Sets

### Step 1: Log in to ConfigCobra

Log in at [app.configcobra.com](https://app.configcobra.com) using your credentials.

### Step 2: Navigate to Rule Sets page

Go to the **Rule Sets** page in the main navigation menu.

### Step 3: Create a new rule set

Here you can create or edit existing rule sets. To create a new one:

1. Press **"Add New Rule Set"** in the top right corner
2. Give a **name** and a **description** for your rule set
3. Select the **controls** that you want to add into the rule set from the available CIS Benchmarks
4. Press **"Add"** to create your rule set

### Step 4: Edit an existing rule set

To edit a rule set, press the **edit icon** on the right side of the desired rule set. You can update the name, description, or modify which controls are included in the rule set.

### Step 5: Delete a rule set

To delete a rule set, press the **delete button** on the right of the desired rule set. This action cannot be undone.

## Best Practices

- **Create rule sets based on compliance requirements** (e.g., SOC 2, ISO 27001, GDPR)
- **Name your rule sets descriptively** to easily identify their purpose
- **Use rule sets in scheduled scans** to ensure consistent monitoring of critical controls
- **Review and update rule sets regularly** as your compliance needs evolve

## Use Cases

### Compliance-Focused Rule Sets
Create rule sets that align with specific compliance frameworks:
- SOC 2 controls
- ISO 27001 requirements
- GDPR data protection controls
- Industry-specific regulations

### Critical Security Controls
Focus on the most important security controls for your organization:
- High-risk controls
- Frequently failing controls
- Controls requiring immediate attention

### Department-Specific Rule Sets
Create rule sets for different departments or teams:
- IT Operations
- Security Team
- Compliance Team
- Executive Dashboard

## Tips

- Start with a small set of critical controls and expand over time
- Review rule set effectiveness regularly
- Combine multiple rule sets in scheduled scans for comprehensive coverage
- Document the purpose of each rule set in the description field

---

[← Back to Documentation](./README.md) | [Next: Scheduled Scans →](./schedules.md)

