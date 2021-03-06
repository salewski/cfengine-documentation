---
layout: default
title: Alerts and Notifications
sorting: 40
published: true
tags: [cfengine enterprise, user interface, mission portal]
---

## Create a New Alert ##

* From the Dashboard, locate the rectangle with the dotted border.

* When the cursor is hovering over top, an **Add** button will appear.


![New Alerts](Alerts.new.png)

* Click the button to begin creating the alert.


![New Alerts Name](Alerts.top.name.png)

* Add a unique name for the alert.

* Each alert has a visual indication of its severity, represented by one of the following colors:
	* **Low**: Yellow
	* **Medium**: Orange
	* **High**: Red
	

![New Alerts Severity](Alerts.top.severity.png)

* From the **Severity** dropdown box, select one of the three options available.
	
* The **Select Condition** drop down box represents an inventory of existing conditional rules, as well as an option to create a new one	


![New Alerts Condition](Alerts.top.condition.png)

* When selecting an existing conditional rule, the name of the condition will automatically populate the mandatory condition **Name** field.

* When creating a new condition the **Name** field must be filled in.


![New Alerts Condition Type](Alerts.bottom.condition.type.png)

* Each alert also has a **Condition type**:
	* **Policy** conditions trigger alerts based on CFEngine policy compliance status. They can be set on bundles, promisees, and promises. If nothing is specified, they will trigger alerts for all policy.

	* **Inventory** conditions trigger alerts for inventory attributes. These attributes correspond to the ones found in inventory reports.

	* **Software Updates** conditions trigger alerts based on packages available for update in the repository. They can be set either for a specific version or trigger on the latest version available. If neither a package nor a version is specified, they will trigger alerts for any update.
	
	* **Custom SQL** conditions trigger alerts based on an SQL query. The SQL query must returns at least one column - `hostkey`.

* Alert conditions can be limited to a subset of hosts.

![New Alerts Hosts](Alerts.bottom.hosts.png)

* Notifications of alerts may be sent by email or custom action scripts.

![New Alerts Notifications](Alerts.bottom.notifications.png)

* Check **Email notifications** box to activate the field for entering the email address to notify.

* The **Remind me** dropdown box provides a selection of intervals to send reminder emails for triggered events.
