# Release Information

- **Version**: 1.0.0

- **Certified**: Yes

- **Publisher**: Fortinet

- **Scope**: Context and Enrichment, Triage

- **Verified with Models**: Fortinet FortiAI (AI model Medium)

# Organizational Context Provider

Retrieves organization-specific information such as business activities, schedules, events, policies, and compliance requirements.

## Installation

This agent installs along with the FortiAI solution pack.

## Configuration

**Required MCP Servers**: NA

<!-- > [!Note]
>
> Refer to [Configuring MCP Servers](https://docs.fortinet.com/document/fortisoar/8.0.0/administration-guide/823139/mcp-servers#Configure_MCP_Servers) on FortiSOAR platform documentation for information on configuring a custom MCP server.
>  -->

### Prerequisites

- The FortiAI solution pack must be installed and configured with the Fortinet FortiAI connector.

  - To configure the FortiAI solution pack, refer to the [FortiAI](https://github.com/fortinet-fortisoar/solution-pack-fortinet-advisor/) solution pack documentation.
  - To configure the Fortinet FortiAI connector, refer to the [Fortinet FortiAI](https://docs.fortinet.com/fortisoar/connectors/fortinet-fortiai) connector documentation.

> [!Note]
>
> FortiAI solution pack and Fortinet FortiAI connector are preconfigured out-of-the-box with FortiSOAR `v8.0.0`.
> 


## Input Parameters

The input must be provided as a JSON object.

| Parameter      | Description                                                       |
|----------------|-------------------------------------------------------------------|
| `question`     | The question that needs to be answered.                           |
| `search_query` | List of queries which will help to search through context memory. |

## Response

The output is returned as a JSON object.

| Parameter    | Description                                                     |
|--------------|-----------------------------------------------------------------|
| `answer`     | Answer to the query derived from available data.                |
| `confidence` | Confidence percentage indicating reliability of the answer (For example: *85%*).     |
| `evidence`   | Supporting information and details from retrieved data sources. |

