---
title: "Schedule Groups"
chapter: true
weight: 20
---

## Schedule Groups

Defining and managing schedules can be cumbersome. To help with this process, use schedules with schedule groups to allow more flexibility in how your organization manages routing hours. Schedules are the blocks of time for which a call route is selected. Schedule Groups allow you to combine multiple schedules and associate them to a singular routing definition. You can assign the schedules into a designated time zone and group them by type. Types are limited to Open Hours, Closed Hours, or Holiday. 

While still under **Routing**, click **Scheduling**. Next, click **Schedules** tab. Click **+Add Schedule.** Let’s name this schedule, “Workshop Open.”

Let’s toggle on the **Repeating Event** and repeat it once per day, since these are our contact centers open hours. We’ll set the time parameters as 7am to 5pm. If you’re going to be testing this flow, be sure to assign hours to your schedule that correspond with your testing. 

![Routing Schedule](/images/Schedule.jpg)

We’ll leave the additional criteria for now, click **Save.**

Return to the **Scheduling** Main Menu and this time create a **Schedule Group** at the top. Click **+Schedule  Group** and name it “Workshop Group”. At the far right, we’ll add a time zone, then under **Schedules,** let’s add one under **Open.**

You’ll see a drop-down appears and we can choose the “Workshop Open,” we previously created. You can add additional time parameters under **Closed** and **Holiday,** but for now let’s save.

Let’s return to our Inbound Call Flow by choosing **Admin > Architect > Inbound Flow > “Workshop – Your Name”.** Now, in our help desk task, open **Logical** in the toolbar. You should see an option for **Evaluate Schedule Group,** drag and drop this at the top of the flow, above **Transfer to ACD.** On the far right, choose the **Schedule Group** as Workshop Group. You’ll now see your flow can branch out based upon the hours of your contact center. While we don’t have to add additional paths here, feel free to add any additional transfer types from the toolbar. 

![Routing Schedule Group](/images/ScheduleGroup.jpg)