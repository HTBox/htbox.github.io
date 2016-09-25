---
layout: default
---

# Development Guidelines

## Conventions and Patterns

### Mediatr Components - Naming Conventions

The project has adopted a CQRS pattern using the Mediatr library. We have discussed ([read discussion](https://github.com/HTBox/allReady/issues/1262)) the naming for these components and agreed that we will *not* suffix them with "Async".

**Commands:**

A command message should end with "Command" and descibe the action that is intended. e.g.

- EditCampaignCommand
- DeleteTaskCommand

The handlers should match the command message name with the suffix of "Handler". e.g.

- EditCampaignCommandHandler
- DeleteTaskCommandHandler

**Queries:**

A query message should end with "Query" and describe the data it returns. e.g.

- EventSummaryQuery
- TaskDetailQuery

The handlers should match the query message name with the suffix of "Handler". e.g.

- EventSummaryQueryHandler
- TaskDetailQueryHandler