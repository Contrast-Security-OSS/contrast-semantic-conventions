# Semantic Conventions for Contrast Actions

Actions are a concept for Security Observability. They are modeled as a metric
so that actions are seen for every requests and collected in a scalable
manner for the agent. We will never miss an action on a particular execution path.

The data used in the action is captured as attributes within a span of a trace. Since capturing and processing spans is considered an expensive activity, this data is captured as part of a sampling activity.

Information in traces allow us to construct an action graph of the execution ordering and also gives us the same data used within an action. However, since they are sampled, its possible to miss some execution paths that execute other actions.  Metrics contain what actions have occurred on an endpoint and are captured for every request, thus they will never miss a particular action.  This fidelity comes at a cost however in that metrics will not contain data used in an
action nor will it contain enough information to determine the action execution order.

<!-- toc -->

- [Actions](#actions)
  * [Metrics](#metrics)
  * [Spans](#spans)
- [Resource additions from Contrast](#resource-additions-from-contrast)

<!-- tocstop -->

## Actions

### Metrics

- [Action Metrics](action-metrics.md): Semantic Conventions for Action metrics.

### Spans

- [Action Spans](action-spans.md): Semantic Conventions for Action spans.

## Resource additions from Contrast

<!-- semconv resource.contrast(full) -->
<!-- NOTE: THIS TEXT IS AUTOGENERATED. DO NOT EDIT BY HAND. -->
<!-- see templates/registry/markdown/snippet.md.j2 -->
<!-- prettier-ignore-start -->
<!-- markdownlint-capture -->
<!-- markdownlint-disable -->


**Status:** ![Experimental](https://img.shields.io/badge/-experimental-blue)

**type:** `contrast`

**Description:** Additional attributes for Contrast Sensors to provide

| Attribute  | Type | Description  | Examples  | [Requirement Level](https://opentelemetry.io/docs/specs/semconv/general/attribute-requirement-level/) | Stability |
|---|---|---|---|---|---|
| [`contrast.deployment`](/docs/attributes-registry/contrast.md) | string | deployment environment | `QA`; `DEVELOPMENT`; `PRODUCTION` | `Recommended` | ![Experimental](https://img.shields.io/badge/-experimental-blue) |
| [`contrast.semconv.version`](/docs/attributes-registry/contrast.md) | string | The version of contrast semantic conventions the data adheres to. | `0.3.0` | `Recommended` | ![Experimental](https://img.shields.io/badge/-experimental-blue) |
| [`otel.semconv.version`](/docs/attributes-registry/contrast.md) | string | The version of otel semantic conventions the data adheres to. | `1.22.0` | `Recommended` | ![Experimental](https://img.shields.io/badge/-experimental-blue) |

`contrast.deployment` has the following list of well-known values. If one of them applies, then the respective value MUST be used; otherwise, a custom value MAY be used.

| Value  | Description | Stability |
|---|---|---|
| `DEVELOPMENT` | development environment | ![Experimental](https://img.shields.io/badge/-experimental-blue) |
| `PRODUCTION` | production environment | ![Experimental](https://img.shields.io/badge/-experimental-blue) |
| `QA` | quality assurance environment | ![Experimental](https://img.shields.io/badge/-experimental-blue) |

<!-- markdownlint-restore -->
<!-- prettier-ignore-end -->
<!-- END AUTOGENERATED TEXT -->
<!-- endsemconv -->
