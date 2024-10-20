# Observability- Part 1: Introduction to Observability

## What is Observability?

Observability is the ability to understand the internal state of a system by analyzing the outputs it produces, such as metrics, logs, and traces. It helps answer critical questions about your system:

- **What is the state of the system?**  
  Understanding resource utilization like CPU, memory, disk I/O, and HTTP requests to determine the current state of your application, infrastructure, and network.
  
- **Why is the system in that state?**  
  By analyzing patterns in logs and system outputs, you can determine why the system is behaving a certain way.
  
- **How will you fix the system's state?**  
  Observability tools provide the data needed to troubleshoot and resolve issues, returning the system to its optimal state.

## The Three Pillars of Observability

Observability is built on three core pillars:

1. **Metrics**  
   Metrics provide quantitative data about the system’s state over time, such as CPU utilization and request rates. They answer the question: *What is the current state of the system?*

2. **Logs**  
   Logs offer detailed, timestamped records of events occurring within the system. They help pinpoint the exact time and nature of issues. Logs answer the question: *Why is the system in this state?*

3. **Traces**  
   Traces track the path of requests through distributed systems, helping engineers debug and troubleshoot issues. They answer the question: *How do you fix the system’s state?*

## Why Do Companies Invest in Observability?

Businesses invest in observability to maintain **Service Level Agreements (SLAs)** and manage **error budgets**. Observability ensures continuous monitoring and feedback on the health of a system, helping to quickly detect and address deviations from SLAs.

## What is an Error Budget?

An **error budget** is the acceptable amount of downtime or failure allowed while still meeting the SLA. For example, if the SLA guarantees 99.9% uptime, the error budget is the 0.1% of downtime permitted over a defined period. Error budgets help teams balance between system reliability and feature development.

## Who is Responsible for Setting Up Observability?

Setting up observability is a collaborative effort between **developers** and **DevOps engineers**. Developers instrument the code to generate metrics, logs, and traces, while DevOps engineers implement and maintain the observability stack.

## Observability Tools

Several tools are used to implement observability across metrics, logs, and traces, including:

- **Prometheus** - Open-source monitoring for metrics collection.
- **Grafana** - Visualizes metrics from sources like Prometheus.
- **Elasticsearch, Logstash, Kibana (ELK Stack)** - For searching, analyzing, and visualizing logs.
- **Jaeger** - Open-source tool for distributed tracing.
- **Datadog** - Full-stack observability platform.
- **New Relic** - Cloud-based platform for end-to-end visibility.

## What is OpenTelemetry?

**OpenTelemetry** is an open-source project that provides APIs, libraries, agents, and instrumentation to collect telemetry data (metrics, logs, and traces) from distributed systems. It standardizes observability across different environments and supports various backends, including Prometheus and Jaeger.

## Observability vs. Monitoring

While related, observability and monitoring serve different purposes:

- **Monitoring** focuses on collecting and visualizing metrics, setting up alerts, and tracking system performance.
- **Observability** goes beyond metrics by incorporating logs and traces, helping engineers diagnose why issues are happening and how to fix them.
