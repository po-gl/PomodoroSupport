---
layout: default
---

### What is Pomodoro?
Pomodoro is a time management technique developed by Francesco Cirillo in the 80s and expanded on in the 90s. The basic idea is to decide what tasks to do at the start of the day and estimate how long they will take; throughout the workday, work for 25 minutes, rest for 5 minutes, then take a more extended 15-30-minute break after repeating the work-rest interval four times. Finally, record how long tasks took and compare against your estimations. The purpose is to be more deliberate about your decision-making, reduce interruptions, and alleviate anxiety associated with the concept of _becoming_ (a concept relating to how we view time). You can read more about the technique in this [paper](http://friend.ucsd.edu/reasonableexpectations/downloads/Cirillo%20--%20Pomodoro%20Technique.pdf).

### Why do live activities require an internet connection?
It’s a limitation on Apple’s current Live Activities api that requires updates to happen through either a background process or a push notification through an external server (which sends the notification via Apple Push Notification service). While updating the live activity through a background process is possible, it is unreliable and wouldn’t run for more than an hour, which is shorter than most Pomodoro sessions. Thus, an external service is used to follow along with your Pomodoro session and update the live activity as the phase changes. Data transmitted to the server is sent via a secure HTTPS connection, including the tasks (title only) and time durations for the current Pomodoro session. No data is saved to the server and only exists on the server for the duration of the service (i.e., the Pomodoro session).

### I've found a bug!
I'd love to hear about it at <a href="mailto:{{ site.email }}">{{ site.email }}</a>

### I'm getting an error message on the task list ⚠️
Send me an email at <a href="mailto:{{ site.email }}">{{ site.email }}</a> and include the error code number if you still have it.
