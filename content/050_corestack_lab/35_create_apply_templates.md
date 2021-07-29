---
title: "2. CoreStack Templates"
chapter: true
weight: 11
---

## Create and apply templates

CoreStack™ also provides the option for users to upload their own templates and use them to execute against their service accounts. Follow the steps given below: Use the ‘+’ button next to the ‘Search’ bar at top right.

Template create window will have 3 sections as follows: Properties, Content and Metadata.

![CoreStack Templates](../images/cs_crtemp1.png "CoreStack Templates")

Lists all template executions of the current tenant. A sample screenshot is shown below. The tabs at the top right represents the archive status of jobs. You can see 2 tabs: Active Jobs and Archived Jobs.​

![CoreStack Templates](../images/cs_crtemp2.png "CoreStack Templates")

### Additional information on Template Actions

Template actions will be shown to every template listed when you are hovering mouse on a template. The list of actions depends on the scope of the template (Marketplace, My Templates) and the RBAC access for templates that user has.

**Execute** – Executes the template immediately and redirects to “Job history” where you can see the status and output of the execution.   

**Edit**– Modifies the properties, content, metadata of the Template. It's like Template Create workflow.   

**Schedules** – Similar to Execute, but schedules it to be run later once/multiple times.  

**Delete** – Deletes the template  

{{% notice tip %}}
**Execute Template**
{{% /notice %}}

Executes the template against [Cloud Accounts](https://docs.corestack.io/manage-cloud-accounts/) and performs the tasks specified in the template. In ‘Job History' you can find the status and outputs for this execution. Execute requires following inputs:  

**Job Name** – Optional. If not given system will generates this.  

**Cloud Account** – Cloud Account need to be used for execution.  

Cloud Account Additional Info – Additional Info of Cloud Account (E.g., Resource Group, Location, Region).  

**Execution Parameters** – Additional parameters from the Template.

A sample Template execute window, for a simple example of taking an `AWS_EC2_Instance_With_SecurityGroup` is shown below:

  ![Template Execution](/images/templaterun.gif)

The [Cloud Accounts](https://docs.corestack.io/manage-cloud-accounts/) lists the available list of AWS cloud accounts in this Tenant

Once the Cloud Account details are selected, click on “Load Execute parameters” to get the input parameters of the template.
