---
title: "Additional Tools"
chapter: true
weight: 10
---
## Additional Tools

#### Import/Export

You can import and export flow configuration. When you import a file, Architect analyzes the file to determine the type of configuration data that it contains. The prompts you are given depend on the type of file it is importing. You can also export a previously created flow’s configuration file for use in another flow. For more information, click to expand the appropriate sections, and click again to close it.
**Note:** Importing a flow from an outside organization may require some configuration updates; even if for items such as data actions with similar names. Until you update any configuration issues, Architect returns validation errors in the flow.

#### Version

You can access a flow's version history from the currently opened flow or from the list of flows on the Architect home page. In the Available Versions dialog box, you can view a list of all available versions of the flow, including:
* Whether a version is published
* The latest working copy
* The latest checked in date of each version, and the author who checked in the flow
When you open a previous version of a flow, you can perform additional tasks. For example, you can unpublish the currently published version. You can also open any version and export the configuration or use Save As to create a copy of the current flow and save it under a new name.

#### Validate

When you configure a flow, Architect checks it to catch problems. If the flow contains errors, the number of errors appears in red or yellow to indicate that you need to update a property action or operation. Red validation errors prevent the flow from working, and must be resolved before Architect implements it for call processing. Yellow validation errors include suggestions or best practice recommendations, but will not prevent the flow from working.
Hover over the **Validate** button. Architect displays a list of validation errors and an explanation of each error.

![Architect Tools](/images/Tools.jpg)

#### Debug

Use the debug feature in Architect to test a separate version of a flow prior to publishing it. This feature lets you listen to the flow from the caller’s point of view by calling it from Genesys Cloud. In debug mode, the flow provides additional system information to the flow author. For example, actions taken or results of decision processes. You can dial a SIP address that specifically calls the flow. The flow to debug cannot contain validation errors. 
To create a debug version of a flow open the **Publish** menu and select **Debug.** The Debug Enabled dialog box opens with confirmation that the flow can be debugged. Copy the flow pattern, open up a phone call from the Genesys Cloud UI, and paste the code as your contact to be called. We’ll use this feature when it is time to test the flow.

![Architect Tools cont.](/images/Debug.jpg)