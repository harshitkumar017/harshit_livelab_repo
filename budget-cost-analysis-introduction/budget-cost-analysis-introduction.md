# Budget and Cost Analysis Introduction

## Budgets Overview
Budget can be used to set soft limits on your Oracle Cloud Infrastructure spending. You can set alerts on your budget to let you know when you might exceed your budget, and you can view all your budgets and spending from one single place in the Oracle Cloud Infrastructure console.

Estimated Lab Time: n minutes

### Budget Concepts
The following concepts are essential to working with budgets:

**BUDGET**
A monthly threshold you define for your Oracle Cloud Infrastructure spending. Budgets are set on cost-tracking tags or compartments and track all spending in the cost-tracking tag or compartment and any child compartments. Note: the budget tracks spending in the specified target compartment, but you need to have permissions to manage budgets in the root compartment of the tenancy to create and use budgets.

**ALERT**
You can define email alerts that get sent out for your budget. You can send a customized email message body with these alerts. Alerts are evaluated every 15 minutes and can be triggered when your actual or your forecasted spending hits either a percentage of your budget or a specified set amount.

[](youtube:uBIOGMqvMos)

### How Budgets Work

Budgets are set on cost-tracking tags or on compartments (including the root compartment) to track all spending in that cost-tracking tag or for that compartment and its children.

All budgets alerts are evaluated every 15 minutes. To see the last time a budget was evaluated, open the details for a budget. You will see fields that show the current spend, the forecast and the "Spent in period" field which shows you the time period over which the budget was evaluated. When a budget alert fires, the email recipients configured in the budget alert receive an email.

## Cost Analysis Overview

Cost Analysis is an easy-to-use visualization tool to help you track and optimize your Oracle Cloud Infrastructure spending, allows you to generate charts, and download accurate, reliable tabular reports of aggregated cost data on your Oracle Cloud Infrastructure consumption. Use the tool for spot checks of spending trends and for generating reports. Common scenarios you might be interested in include:

Show monthly costs for compartment X and its children, grouped by service or by tag.
Show daily costs for tag key A and tag key B, values X, Y and Z, grouped by service and product description (SKU).
Show hourly costs for service = compute or database, grouped by compartment name.
You can choose the dates you’re interested in. Filter to the specific tags, compartments, services, or filter you want, and pick how you want it grouped. As a result, a chart and corresponding data table are generated, and can also be downloaded as a data table.

If you want to re-create the breakdown provided by the Classic Version in the Latest Version of the Cost Analysis tool, apply the SKU (Part Number) grouping dimension. To explore your costs in new ways, we recommended viewing your costs based on Service, or Service and Product Description. If you are doing cost tracking, we recommended grouping by Compartment or Tag.

### How Cost Reports Work

The cost report is automatically generated daily, and is stored in an Oracle-owned Object Storage bucket. It contains one row per each Oracle Cloud Infrastructure resource (such as instance, Object Storage bucket, VNIC) per hour along with consumption information (usage, price, cost), metadata, and tags. Cost reports generally contain 24 hours of usage data, although occasionally a cost report may contain late-arriving data that is older than 24 hours.

Cost reports may contain corrections. Corrections are added as new rows to the report, with the lineItem/iscorrection column set and the referenceNo value of the corrected line populated in the lineItem/backReference column.

Cost reports are retained for one year.

The file name for each cost report is appended with an automatically incrementing numerical value.


## Learn More


* [Budget](https://docs.cloud.oracle.com/en-us/iaas/Content/Billing/Concepts/budgetsoverview.htm)
* [Cost Analysis](https://docs.cloud.oracle.com/en-us/iaas/Content/Billing/Concepts/costanalysisoverview.htm)

## Acknowledgements
- **Authors/Contributors** - Harshit Kumar, Constantin Sebe
* **Last Updated By/Date** - Harshit Kumar, August 2020 <Name, Group, Month Year>

## See an issue?
Please submit feedback using this [form](https://apexapps.oracle.com/pls/apex/f?p=133:1:::::P1_FEEDBACK:1). Please include the *workshop name*, *lab* and *step* in your request.  If you don't see the workshop name listed, please enter it manually. If you would like for us to follow up with you, enter your email in the *Feedback Comments* section.
