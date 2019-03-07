Incident - A chronological view of one or more violations that includes timestamps for each violation and chart snapshots of the data being evaluated for the time of each violation. 

Thresholds - The min or max values and frequency level for an alert condition that will trigger an alert notification and open an incident when violated. 

Notification Channel - A designated destination for sending alerts when incidents are opened, acknowledged, or closed

Alert Conditions - The specific type of events in an app will trigger an alert for the selected policy

Alert Policy - A list of collection of alert conditions and notification channels that applies to a single New Relic product and a specific app(s) or key transaction(s)

Thresholds - The mix/max values and frequency for the alert condition that will trigger an alert when violated

Warning Threshold - Want to monitor, but don't want notifications

Webhook - Generic notification that can post to any channel

Critical Threshold - Triggers notification when it exceeds the threshold for the set period of time

Alert policies don't need notification channels

Critical thresholds must be set, warnings don't need to be set

Must select a specific entity or it will be set to nothing

Must select a new relic product and the type of conditions vary based on product you select

