# Cloud Resiliency and Availability

## Availability

- Understand and Calculate the overall compound availability
  - https://megamorf.gitlab.io/cheat-sheets/calculate-compound-availability/
  - > Note: pay special attention to dependent services that may be on-prem
- Design for high availability
  - Leverage PaaS services
  - Deploy two or more VMs to achieve the required SLA
  - Deploy to two or more regions
  - Leverage availability-zones (higher availability in the same region)

## Resilency

- Build for self-healing
- Implement Resient Patterns
  - Retry
  - Circuit breaker
- Implement Resilient Architectures
  - If main service fails, write to a backup service (ie write to ServiceBus if you cannot write to SQL)
  - Choose higher availability services (i.e. Cosmos DB 99.999%)

## Monitor and Alerting

- Implement monitor and alerting

## Reference Document

- https://docs.microsoft.com/en-us/azure/architecture/guide/design-principles/
