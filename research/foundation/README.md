<samp>

# Distributed Tracing Concept

Distributed Tracing is a way to track requests in applications as they flow in a distributed system (e.g, Microservices) that communicate using various protocols (e.g, HTTP/HTTPS, Message Queue)

### Benefits:
* Accelerate software troubleshooting
* Improve developer collaboration
* Reduce time to market

### Different types:
* Code tracing
* Program tracing
* End-to-end tracing

### Components
* Trace - complete path of request, consisting multiple spans
* Span - single unit of work within a trace (e.g, function call, database query)
* Trace context - information passed to link spans across different services, includes trace ID and span ID
* Context propagation - mechanism of passing trace context across different services to link spans
* Instrumentation - adding code to an application to generate trace data (spans)
* Sampling - technique to reduce the amount of trace data by selecting a sample request
* Visualization & distributed tracing tools options:
  * OpenTelemetry - collection of APIs, SDKs, and tools, to instrument, generate, collect, and export telemetry data (metrics, logs, and traces)
  * AWS X-Ray - monitor, visualize, and debug distributed applications
  * 

![](https://github.com/user-attachments/assets/9a296fa3-c01d-4d79-913e-ad70615531f8)
:--:
*[Image Source](https://docs.logz.io/docs/user-guide/distributed-tracing/tracing-overview/what-tracing/)*

### Standards:
Standardizing distributed tracing workflow. Common framework and software tools for developers (monitor, visualize, and analyze service request), also prevents vendor lock-in
* OpenTracing - provides APIs and instrumentation for distributed tracing
* OpenCensus - provides APIs and instrumentation that allow you to collect application metrics and distributed tracing
* OpenTelemetry - new effort to combine distributed tracing, metrics, and logging (combines the best of OpenTracing + OpenCensus)

### Difference between logging and distributed tracing:
* Logging - record specific event and only tells what happened in an application
* Distributed Tracing - provides an audit trail, focused on why an incident occurred by correlating various telemetry data, may use logging and other data to trace specific service request

### Challenges
* Manual instrumentation - risks of coding errors that affect production releases
* Limited frontend coverage 
* Random sampling

***
WIP...
</samp>
