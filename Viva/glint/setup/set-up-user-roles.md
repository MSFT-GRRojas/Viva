---
title: Set up Viva Glint User Roles
description: Admins assign roles, edit roles, and can export and import roles manually or in bulk for their Viva Glint programs.
ms.author: JudithWeiner
author: JudyWeiner
manager: MelissaBarry
audience: admin
f1.keywords: NOCSH
keywords: permissions, bulk imports, user role imports, custom access, status change, active, inactive 
ms.collection: 
 - m365initiative-viva
 - selfserve
search-appverid: MET150
ms.topic: article
ms.service: viva-glint
ms.localizationpriority: high
ms.date: 08/07/2024
---

# Set up Viva Glint User Roles

Admins can assign multiple roles with specific permissions - access to different segments of data and filters - in **User Roles**. 

:::image type="content" source="../../media/glint/setup/user-roles-access.png" alt-text="Screenshot that shows how to access User Roles from the admin dashboard.":::

## Glint User Role template

Use the template as a planning tool to define permissions for roles, according to these three filter distinctions:

- **Report filters**: Attributes the role can use to filter results
- **Report sections**: Attributes the role can use to add sections in reports
- **Comment filters**: Attributes the role can use as filters to review comments

The [**User Roles and Access template**](https://www.microsoft.com/download/details.aspx?id=105793) includes prepopulated example roles and instructions for defining permissions. 

**Not all User Roles and prepopulated attributes and permissions in the template may apply to your organization. Use your Employee Attribute File for attributes specific to your organization to customize your template.**

> [!TIP]
> To protect confidentiality, give managers access to only one filterable attribute. Assigning more than one filterable attribute increases the chance that a manager can deduce the origin of individual responses.

## Default User Roles

The following roles are preconfigured in Glint and can't be edited. Create a new User Role with a new name if you want to edit these attributes and permissions.

- **Company Admin**: Employees who are granted **ALL** permission; can't be edited. Includes Advanced Configuration access.
- **Active Employees**: Not intended to have data access.
- **Inactive Employees**: Not intended to have data access.
- **Managers**: Doesn't allow edits, create a different manager role to change permissions and attributes
- **Support Users**: [External users](https://go.microsoft.com/fwlink/?linkid=2240483) who have advanced access; can't be edited. 

## Enable User Roles

Admins can specify the employee population and attributes their leaders can view on their dashboard for each User Role. Defining roles is important for data cuts, access permissions, and program integrity.

1. Select the **Configuration** symbol.
1. In the **Employees** section, select **User Roles**.
1. Select **+New Role**. The **Role Settings** page displays.
1. Enter a role name in the **Untitled Role** field by selecting the **pencil** symbol.

   :::image type="content" source="../../media/glint/setup/user-roles-title.png"alt-text="Screenshot of the Role Settings page.":::

1. Select **Permissions**.

   :::image type="content" source="../../media/glint/setup/user-roles-access-permissions.png" alt-text="Screenshot of Access Permissions in Role Settings.":::

1. Make choices for these sections based on decisions in your User Role template:
   1. Survey Programs
   
      :::image type="content" source="../../media/glint/setup/user-roles-survey-programs.png" alt-text="Screenshot of the Survey Programs Access section in Permissions and Access.":::

   1. Focus Areas and Conversations
   
      :::image type="content" source="../../media/glint/setup/user-roles-focus-areas-convos.png" alt-text="Screenshot of the Focus Areas and Conversations section in Permissions and Access.":::

   1. Reporting
   
      :::image type="content" source="../../media/glint/setup/user-roles-reporting.png" alt-text="Screenshot of the Reporting section in Permissions and Access.":::

   1. Data Management
   
      :::image type="content" source="../../media/glint/setup/user-roles-data-management.png" alt-text="Screenshot of the Data Management section in Permissions and Access.":::

   1. Resources
   
      :::image type="content" source="../../media/glint/setup/user-roles-resources.png" alt-text="Screenshot of the Resources section in Permissions and Access.":::

   1. Access Permissions
   
      :::image type="content" source="../../media/glint/setup/user-roles-access-permissions-section.png" alt-text="Screenshot of Access Permissions window.":::

1. Select **Save Changes**.

1. On the **Role Settings** page, select **Report Attributes**.

   :::image type="content" source="../../media/glint/setup/user-roles-report-attributes.png" alt-text="Screenshot of Report access in Role Settings.":::

1. Attributes are separated into sections:
    - Standard
    - Manager Hierarchy: Select all levels, for roles with Manager Hierarchy-based access, users see only their team
    - Other Reporting Hierarchies: For instance, Location or Department Hierarchy

1. Select all attributes and hierarchies that this role should be allowed to view:
    - Report filters
    - Report sections
    - Comment filters

1. Select **Save Changes**.

> [!TIP]
> Filtering through results across too many attributes makes identifying survey respondents easier. For this reason, it's best to give access to only one attribute per manager role. 

## Add or edit employees in a role

Select the **Add/Edit Employees** button. The **Choose a way to add employees** window opens.

Add members to a User Role by choosing from these options:

- **Attribute Rules**: [User rules](#attribute-rule-based-user-roles) like Location or Department to populate a User Role. This dynamically changes with your employee data uploads.
- **Import**: Use a CSV or XLSX file to [import employees](#import-user-roles-in-bulk) for this User Role. 

> [!IMPORTANT]
> - Switching from **Attribute Rules** to **Import** removes attribute rules.
> - Switching from **Import** to **Attribute Rules** overrides any employees uploaded.
   
### Attribute rule-based User Roles

:::image type="content" source="../../media/glint/setup/user-roles-attribute-slider.png" alt-text="Screenshot of the **Add Attribute Rules** section in Role Settings.":::

1. From your admin dashboard, choose the **Configure** symbol and then select **User Roles**.  
2. Choose any role - *excluding preconfigured roles*.
3. Select  **Add/Edit Employees.**
4. In the new display window, choose either:
   - I want to include all active employees only, or
   - I want to filter all active employees by the following populations

5. To add users based on a filtered population, select  **I want to filter all active employees by the following populations**.
6. Select  **+ New Population**.
7. Select  **+ Add Filter**  to select an attribute to filter your employee list. Your attribute list is unique to your organization based on your Employee Attribute File.
8. Select  **Done**.
9. To exclude someone, search their name and select **Exclude**.
10. To remove someone from the Excluded list, search their name and select **Remove**.
11. Confirm list for User Role and select  **Save Changes**.

## Import User Roles in bulk

When you need to assign many individuals to a specific User Role, use the bulk import feature.

:::image type="content" source="../../media/glint/setup/user-roles-import-dialog-box.png" alt-text="Screenshot of the Import Employees to Role dialog box in Role Settings.":::

1. From your admin dashboard, choose the **Configure** symbol and then select **User Roles**.
2. On the **Role Settings** page, select **Export.** In the window that opens, make your selections and select **Export**.
3. Open the downloaded CSV file and delete all columns except the column with email addresses.
4. Add or delete email addresses, as needed. This can be a full replacement for the existing file, so you won't need to have an *Add* or *Remove* column.
5. Save your file.
1. Return to the **Role Settings** page and select **Import**.
1. Select the checkbox to indicate if you only added users.
1. Drag and drop your file, or browse to select your file, into the area indicated.
1. Select **Import File**.
1. Confirm your import and select **Confirm Import**.

## Remove a user from a User Role

1. Hover over a user's name.
2. Select the **trash can** symbol.
3. Select **Yes, Remove**.
   
## View and edit attribute rules for a User Role

This functionality works for roles which already have filters and/or populations applied to them.

1. From the **User Roles** page, select a role to view or edit.
2. On the **Role Settings** page, the number of members of this group displays and the attribute rule applies. (Example: *Includes: Gender: Female*)
3. To change, select **Edit Attribute Rules**.
4. In the new display window, choose from:
   - I want to include all active employees only, or
   - I want to filter all active employees by the following populations
5. Add new populations and filters, as desired.
6. Choose whether to include inactive employees or to exclude any employees.
7. Select **Save Changes**.

### Change a User Role status

To change a User Role from ACTIVE to INACTIVE or vice versa, include the users in an upload file with their status changed to "**ACTIVE**" or "**INACTIVE.**" This edit can't be made within the **User Roles** feature. 

## Grant custom access
 
Custom access is intended for users who need to have their default access overridden or are in a role that is so specific, it needs to be *per user* rather than at the User Role level. For example, use custom access for HRBPs who serve unique combinations of employee groups in your organization. To grant custom access in bulk to multiple users for survey, Focus Area, and Admin access, see: [Advanced Configuration uploads](advanced-config-uploads.md).


