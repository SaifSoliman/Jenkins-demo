How webhook differ from poll SCM?

A server makes webhook requests, and a client makes polling requests. Polling is scheduled to run at predetermined intervals regardless of whether there are any new events, but webhooks are activated automatically whenever an event takes place.

When to use Poll SCM?

Polling can be used when real-time updates are not required, as they cause frequent changes in data and can cause your system to crash if you choose to receive updates every time something changes.

Assume you’re running a successful startup with 100 new users joining every second. You want a large screen in the centre of the office that displays your current subscriber count. Subscribing to new data every time a new user signs up would be chaotic.

You should poll your server every five to ten minutes to get the current total number of users. This would reduce your system’s workload and, as a result, its resource consumption.
