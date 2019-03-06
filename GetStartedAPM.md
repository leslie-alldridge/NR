New Relic APM (Application Performance Monitoring)

Collecting data by app name allows aggregration

Without a name, it will obtain a default name

Change name after install requires a name change or add an alias

Change app name
- Reports under new heading
- Determines how aggregation works
- set seperate thresholds 

Change app alias 
- Keeps continuity of data (reports the same)
- Change how the app name appears in APM and Browser
- Organise apps differently 

Data for each instance and aggregated data
- Order from most specific to least specific
- e.g. Individual application instance [number] all send data to Data Center West and we aggregate this via Global Data Center
- The yaml file follows this same naming order convention

New Relic Node API allows you to customise start/end of transactions and customize the app further

Apdex T threshold sets the performance alert score. Satisfied, tolerating and frustrated are the results for good, medium and bad performance. 

Appdex T set to 0.5 means that 2s transactions are tolerating and anything over 2 seconds is frustrated (because it's over 4x more)

Categories and labels can be used to find specific apps and create aggregates. Any apps in a category without data = grey bar. If they have no alerts then they won't be counted in the health check. 

Format is Category:Label e.g. Analytics:Label1   you cannot use spaces or any other special characters. First letter must be capatalized. To use multiple the format is Front-End or Front_End but it'll be saved as Front_end

Removing a label only unassigns it, the label will still be available in the app and search. To permanently remove, you can use the Rest API Explorer.

Alerts can be set up to send notifications to the right people. 
1. Why do you want to be alerted? response times, errors?
2. What criteria will trigger an alert? error percentage, response time, throughput?
3. At what level those conditions will escalate into alerting situations? - thresholds 
4. Who needs to be notified and how will they be notified (Channels)