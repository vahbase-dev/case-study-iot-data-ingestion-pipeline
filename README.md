# IoT Data Ingestion Pipeline — Case Study (Docs-only)

![Cover](./cover.png)

## Overview
A high-throughput ingestion pipeline for industrial IoT sensors using MQTT, designed for reliable delivery, scalable processing, and deterministic downstream storage.

## What I Built
- MQTT ingestion layer with authenticated device sessions
- Stream processing flow for validation, enrichment, and routing
- Backpressure and retry strategy for bursty sensor traffic
- Deterministic event model for replay-safe processing
- Observability plan for end-to-end visibility

## Key Outcomes
- Sustained high ingest under burst traffic using buffering and backpressure controls
- Improved data quality via schema validation and enrichment gates
- Enabled replayable processing with idempotent consumers and stable event ids

## Architecture Highlights
- **Ingress:** MQTT broker + device auth
- **Processing:** stream workers + routing rules
- **Buffering:** queues/streams for backpressure
- **Storage:** time-series + relational projections (implementation-dependent)
- **Operations:** metrics, tracing, alerting, runbooks

## Docs
- [00 — Index](./docs/00-index.md)
- [01 — MQTT Ingress and Device Identity](./docs/01-mqtt-ingress-and-device-identity.md)
- [02 — Stream Processing and Routing](./docs/02-stream-processing-and-routing.md)
- [03 — Storage Model and Projections](./docs/03-storage-model-and-projections.md)
- [04 — Reliability and Backpressure](./docs/04-reliability-and-backpressure.md)
- [05 — Observability and Operations](./docs/05-observability-and-operations.md)

## Notes
This repository is documentation-only and contains no proprietary source code.
