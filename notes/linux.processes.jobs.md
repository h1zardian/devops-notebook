---
id: 7jrrtuzm3n54rlfvm8aassg
title: Jobs
desc: ''
updated: 1657813958975
created: 1650467559384
---

### Background and Foreground Jobs

- Jobs can be run as foreground as well as background processes.

- A job can be sent to the background by suffixing `&` to the command. eg: `updatedb &`.

- Use `ctrl+z` to suspend or `ctrl+c` to terminate a foreground job.

- `bg` and `fg` commands can be used to run a process in background or foreground when suspended or with PID.

### Managing Job

- `jobs -l` provides the same information as `jobs` with added **PID** of the background jobs.
