---
id: 8991mmbcjo38efoqmjk0i3v
title: Process Termination
desc: ''
updated: 1657814025432
created: 1650025651544
---

To terminate a process, you can use
> `kill -9 <pid>`

`kill` -signal_number list:

<pre>
    0     0       (it isn't a valid signal, but can be used to test whether the PID specifies a processes to which a signal could be sent.)
    1     SIGHUP
    2     SIGINT
    3     SIGQUIT
    6     SIGABRT
    9     SIGKILL  (used to kill a process)
    14    SIGALRM
    15    SIGTERM
</pre>

>Process numbers (`PID`) can be found by using [[ps|linux.processes#ps]].
