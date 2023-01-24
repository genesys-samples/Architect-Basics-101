---
title: "Flow Build"
chapter: true
weight: 20
---

## Flow Build

Typically, the first step in a call flow will be identifying our customer. This will be done with a Data Call either via Data Action into a CRM or a Data Table Lookup to pull the customer record. This will push relevant information about the customer to an agent to help guide the customer journey. Audio prompts may also be used along the path to greet or guide the customer. Variable tied to the customer record may be presented here. For example, the flow could reference the customers name to play in a customized audio prompt. Once a customer is identified, deciding what is to be presented to the agent is done with a screen pop. Genesys Cloud CX offers a native scripting tool to build configurable scripts or may reference 3rd party integrations to display the customer record to the agent. 

Our goal in this tutorial, is to push the inbound call directly to the agent. This can be done with **Transfer > Transfer to ACD**. Like the **Task** earlier. This can be dragged and dropped onto the flow timeline. 

Next, we’ll reference the queue our agent belongs to. If you have yet to set up a queue, you may follow the steps here, https://help.mypurecloud.com/articles/create-queue/

![Transfer to ACD](/images/Transfer.jpg)

**Note: Red validation errors prevent a flow from publishing and must be resolved before Architect implements it for call processing. Yellow are suggestion or best practice recommendations, but do not prevent a flow from working.**

You’ll notice our **Pre-Transfer** and **Failed Transfer** audio prompts are marked in yellow. While the flow will still publish, we can get rid of these by providing typing in a prompt for each. Type, “transferring”, in the **Pre-Transfer Audio** and “failed to transfer” in the **Failed Transfer Audio**. You should no longer have yellow validation markers. 

Finally, one red validation marker should remain. This is because if the flow is unable to successfully connect to a queue, the path has no other place to go. We can solve this by providing a **Disconnect** node, jump to another menu or task, or create a loop. For todays workshop, let’s drag and drop a **Disconnect** from the toolbar.

We’re ready to **Save & Publish**

![Transfer to ACD](/images/Validate.jpg)
