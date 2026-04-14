# Architecture Documentation

## Overview
This RAG implements Quality Inspector • BOM (Discrete) for Manufacturing use cases.

## Components
1. **Inspection Intake**: Collect, validate and normalize downtime events from CMMS; attach a runId and timestamp for traceability.
2. **Retrieve**: Execute retrieve phase for the RAG pattern: persist interim state, enforce guardrails, and emit structured JSON results.
3. **Ground**: Execute ground phase for the RAG pattern: persist interim state, enforce guardrails, and emit structured JSON results.
4. **Dispatch**: Dispatch across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
5. **Defect Detection**: Defect Detection across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
6. **Maintenance Plan**: Maintenance Plan across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
7. **Setup Optimization**: Setup Optimization across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
8. **Traceability**: Traceability across joined datasets; branch on thresholds using decision gates; write metrics (success/error counts) for observability.
9. **Maintenance Ticket**: Assemble final payload with status, artifacts, KPIs and audit trail; store to PLM; return response JSON for the client.

## Data Flow
- Input: Inspection Intake
- Processing: 9 sequential steps
- Output: Maintenance Ticket
