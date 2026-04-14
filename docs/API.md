# API Documentation

## Endpoints
### Inspection Intake
- **Description**: Collect, validate and normalize downtime events from CMMS; attach a runId and timestamp for traceability.
- **Type**: Processing

### Retrieve
- **Description**: Execute retrieve phase for the RAG pattern: persist interim state, enforce guardrails, and emit structured JSON results.
- **Type**: Processing

### Ground
- **Description**: Execute ground phase for the RAG pattern: persist interim state, enforce guardrails, and emit structured JSON results.
- **Type**: Processing

### Dispatch
- **Description**: Dispatch across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Defect Detection
- **Description**: Defect Detection across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Maintenance Plan
- **Description**: Maintenance Plan across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Setup Optimization
- **Description**: Setup Optimization across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Traceability
- **Description**: Traceability across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
- **Type**: Processing

### Maintenance Ticket
- **Description**: Assemble final payload with status, artifacts, KPIs and audit trail; store to PLM; return response JSON for the client.
- **Type**: Processing
