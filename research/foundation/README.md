<samp>

# Distributed Tracing Concept

Distributed Tracing is a way to track requests in applications as they flow in a distributed system (e.g, Microservices) that communicate using various protocols (e.g, HTTP/HTTPS, Message Queue)

## Benefits
* Accelerate software troubleshooting
* Improve developer collaboration
* Reduce time to market

## Different types
* Code tracing
* Program tracing
* End-to-end tracing

## Components
### Trace
Complete path of request, consisting multiple spans
![image](https://github.com/user-attachments/assets/5de35428-08d8-407f-ac32-2f61601cb8cf)
:--:
*Sample Trace: [Image Source](https://signoz.io/blog/distributed-tracing-span/)*

### Span
Single unit of work within a trace (e.g, function call, database query, calls to another service, etc.)

### Trace context
Information passed to link spans across different services, includes trace ID and span ID

### Context propagation
Mechanism of passing trace context across different services to link spans

### Instrumentation
Adding code to an application to generate trace data (spans)

### Sampling
Technique to reduce the amount of trace data by selecting a sample request

### Visualization tool
To monitor, visualize, and debug distributed applications, observability tool (e.g, AWS X-Ray, Datadog, SigNoz)

### Distributed tracing tool
Collection of APIs, SDKs, and tools, to instrument, generate, collect, and export telemetry data (metrics, logs, and traces) (e.g, OpenTelemetry)

## Standards
Standardizing distributed tracing workflow. Common framework and software tools for developers (monitor, visualize, and analyze service request), also prevents vendor lock-in
* OpenTracing - provides APIs and instrumentation for distributed tracing
* OpenCensus - provides APIs and instrumentation that allow you to collect application metrics and distributed tracing
* OpenTelemetry - new effort to combine distributed tracing, metrics, and logging (combines the best of OpenTracing + OpenCensus)

## Difference between logging and distributed tracing
Logging record specific event and only tells what happened in an application. In contrast, distributed tracing provides an audit trail, focused on why an incident occurred by correlating various telemetry data, may use logging and other data to trace specific service request

## Challenges
* Manual instrumentation - risks of coding errors that affect production releases
* Limited frontend coverage 
* Random sampling

***
WIP...
</samp>
