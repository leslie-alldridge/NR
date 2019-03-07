REST API - Interact with data stored in NR and change settings
APM Agent API - Control the agent and record data through the agent

Insights - events: whole new event type with associated attributes

Insights & APM: Attributes - additional key pairs to existing transaction traces and error rates

APM: Adding timing data to methods and transactions usually, in order to dig deeper into a transaction.


APM Agent API
- shorter, easier code
- fewer connections
- maintained by NR engineers
- reliable and resilient
- records less data 

Insights Insert API
- Record any data source
- data sent when you want it
- you maintain the code
- highly flexible and customizable, but reliability is up to you
- records more data than APM API

Troubleshooting
1. agent version check to ensure custom event insights are enabled
2. high security mode - if its on custom events won't log
3. check logs - helpful logs to see what went from. Default level is info but you can set to debug or audit for more information
4. config file limit - check max events limit in config.yaml file (1mb is the single file size limit)
5. Check format and types (id cannot be string, etc) Nr. invalid attribute count will populate if this is the case