# uptime-watch

Checks every 5 minutes that https://uptime.mnori.com (Uptime Kuma, which monitors the nj1/nj2 servers) answers.
The first failed check after a good one fails the workflow run, and GitHub emails the repository owner.
Later failures stay quiet until Kuma answers again, so one outage sends one mail.
