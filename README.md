# Financial Remedy Cron Helm Chart

Helm chart for the Financial Remedy kubernetes cron job. It uses the [finrem-case-orchestration-service](https://github.com/hmcts/finrem-case-orchestration-service) image to execute scheduled tasks by passing the arguments: `run [taskname]` to the jar.
