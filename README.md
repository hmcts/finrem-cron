# Financial Remedy Cron Helm Chart

Helm chart for the Financial Remedy kubernetes cron job. It uses the [finrem-case-orchestration-service](https://github.com/hmcts/finrem-case-orchestration-service) image to execute scheduled tasks by passing the arguments: `run [taskname]` to the jar.

# # Notes
When releasing a new version of the chart, ensure the version is updated in both:
- Chart.yaml
- cnp-flux-config
It requires to create a new tag to trigger the build on Azure pipeline. The chart is published to Azure Container Registry (ACR) under helm/finrem-cron with the same version as the tag.
