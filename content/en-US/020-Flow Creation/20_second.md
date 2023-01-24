---
title: "Starting Menu"
chapter: true
weight: 20
---

## Starting Menu

When you begin, your starting menu will consist of two nodes, **Main Menu** and **Disconnect**. If you select Main Menu, you have the option to set up an **Initial Greeting** and **Menu Prompt**. This is the audio prompt and options available your customers will hear when they dial into your contact center. We’ll use Architect’s text-to-speech for our tutorial, but you also have the ability to upload pre-recorded audio prompts to the flow. 

In the toolbox to the right, you’ll see both **Menu** and **Task**. A **Menu** action allows you to create a sub-menu. Here is where you will assign common settings such as DTMF and speech recognition per option. Use the **Task** action to build complex IVR options. A task action groups related steps of a process together to create a flow routine. A process is made up of the tasks involved, the sequence of those tasks, and the actions that exist between them. A **Task** will use the same DTMF and Speech Recognition capabilities as **Menus**. 

![Setting up Main Menu](/images/Menu.jpg)

In our toolbar, Click **Task**, there you’ll find our submenu of task options. Our Architect tools use drag-and-drop functionality for ease of use. Click the submenu item **Task** and drag it under **Disconnect** in our **Main Menu**. Drop it there. Now we can add the DTMF as “1”, and type “One” in our **Speech Recognition** field. Now our customers may reach this task by either hitting the one key on their phone, or simply saying, “one.” Let’s also click on the task heading, currently titled, “New Task 1.” Let’s rename this, “Help Desk.” 

You’ll notice on the left; our task has a red icon next to it. We’ll return to complete this task in the next module and show what the red icon represents and how to fix it. 

![Menu Options](/images/MenuOptions.jpg)