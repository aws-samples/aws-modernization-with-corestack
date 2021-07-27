---
title: "5. Additional workshop specific requirements"
chapter: true
weight: 18
---

## Additional workshop specific requirements

{{% notice tip %}}
**Template Actions​**
{{% /notice %}}

Template actions will be shown to every template listed when you are hovering mouse on a template. The list of actions depends on the scope of the template (Marketplace, My Templates) and the RBAC access for templates that user has.​

**Execute** – Executes the template immediately and redirects to “Job history” where you can see the status and output of the execution.  ​

**Edit**– Modifies the properties, content, metadata of the Template. It's like Template Create workflow.  ​

**Schedules** – Similar to Execute, but schedules it to be run later once/multiple times. ​

**Delete** – Deletes the template ​

{{% notice tip %}}
**Execute Template​**
{{% /notice %}}

Executes the template against [Cloud Accounts](https://docs.corestack.io/manage-cloud-accounts/) and performs the tasks specified in the template. In ‘Job History' you can find the status and outputs for this execution. Execute requires following inputs: ​

**Job Name** – Optional. If not given system will generates this. ​

**Cloud Account** – Cloud Account need to be used for execution. ​

Cloud Account Additional Info – Additional Info of Cloud Account (E.g., Resource Group, Location, Region). ​

**Execution Parameters** – Additional parameters from the Template.​

A sample Template execute window, for a simple example of taking an `AWS_EC2_Instance_With_SecurityGroup` is shown below:​

  ![Template Execution](/images/templaterun.gif)

The [Cloud Accounts](https://docs.corestack.io/manage-cloud-accounts/) lists the available list of AWS cloud accounts in this Tenant​

Once the Cloud Account details are selected, click on “Load Execute parameters” to get the input parameters of the template.
