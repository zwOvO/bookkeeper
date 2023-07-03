---
id: metrics
title: Metric collection
---

BookKeeper enables metrics collection through a variety of [stats providers](#stats-providers).

## Stats providers

BookKeeper has stats provider implementations for these sinks:

Provider | Provider class name
:--------|:-------------------
[Codahale Metrics](https://mvnrepository.com/artifact/org.apache.bookkeeper.stats/codahale-metrics-provider) | `org.apache.bookkeeper.stats.CodahaleMetricsProvider`
[Prometheus](https://prometheus.io/) | `org.apache.bookkeeper.stats.prometheus.PrometheusMetricsProvider`
[OpenTelemetry Metrics](https://opentelemetry.io/docs/specs/otel/metrics/) | `org.apache.bookkeeper.stats.otel.OtelMetricsProvider`

> The [Prometheus]({{ site.github_master }}/stats/bookkeeper-stats-providers/prometheus-metrics-provider) stats provider is the default provider.

## Metrics Provider Settings
See [Statistics settings](../reference/config/#statistics).
