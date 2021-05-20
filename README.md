# Cloud Resiliency and Availability

## Availability

- Understand and calculate the overall compound availability
  - https://megamorf.gitlab.io/cheat-sheets/calculate-compound-availability/
  - > Note: pay special attention to dependent services that may be on-prem
- Design for high availability
  - Leverage PaaS services
  - Examples:
    - Deploy two or more VMs to achieve the required SLA
    - Deploy to two or more regions
    - Leverage availability-zones (higher availability in the same region)
    - Choose higher availability services (i.e. Cosmos DB 99.999%)

## Resilency

- Build for self-healing
- Implement Resient Patterns
  - Incremental retry backoff strategy
  - Circuit breaker
- Implement Resilient Architectures
  - If main service fails, write to a backup service (ie write to ServiceBus if you cannot write to SQL)
  

## Monitor and Alerting

- Implement monitor and alerting

## Reference Document

- https://docs.microsoft.com/en-us/azure/architecture/guide/design-principles/
