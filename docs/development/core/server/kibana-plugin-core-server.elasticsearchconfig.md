<!-- Do not edit this file. It is automatically generated by API Documenter. -->

[Home](./index.md) &gt; [kibana-plugin-core-server](./kibana-plugin-core-server.md) &gt; [ElasticsearchConfig](./kibana-plugin-core-server.elasticsearchconfig.md)

## ElasticsearchConfig class

Wrapper of config schema.

<b>Signature:</b>

```typescript
export declare class ElasticsearchConfig 
```

## Constructors

|  Constructor | Modifiers | Description |
|  --- | --- | --- |
|  [(constructor)(rawConfig)](./kibana-plugin-core-server.elasticsearchconfig._constructor_.md) |  | Constructs a new instance of the <code>ElasticsearchConfig</code> class |

## Properties

|  Property | Modifiers | Type | Description |
|  --- | --- | --- | --- |
|  [apiVersion](./kibana-plugin-core-server.elasticsearchconfig.apiversion.md) |  | <code>string</code> | Version of the Elasticsearch (6.7, 7.1 or <code>master</code>) client will be connecting to. |
|  [customHeaders](./kibana-plugin-core-server.elasticsearchconfig.customheaders.md) |  | <code>ElasticsearchConfigType['customHeaders']</code> | Header names and values to send to Elasticsearch with every request. These headers cannot be overwritten by client-side headers and aren't affected by <code>requestHeadersWhitelist</code> configuration. |
|  [healthCheckDelay](./kibana-plugin-core-server.elasticsearchconfig.healthcheckdelay.md) |  | <code>Duration</code> | The interval between health check requests Kibana sends to the Elasticsearch. |
|  [hosts](./kibana-plugin-core-server.elasticsearchconfig.hosts.md) |  | <code>string[]</code> | Hosts that the client will connect to. If sniffing is enabled, this list will be used as seeds to discover the rest of your cluster. |
|  [ignoreVersionMismatch](./kibana-plugin-core-server.elasticsearchconfig.ignoreversionmismatch.md) |  | <code>boolean</code> | Whether to allow kibana to connect to a non-compatible elasticsearch node. |
|  [logQueries](./kibana-plugin-core-server.elasticsearchconfig.logqueries.md) |  | <code>boolean</code> | Specifies whether all queries to the client should be logged (status code, method, query etc.). |
|  [password](./kibana-plugin-core-server.elasticsearchconfig.password.md) |  | <code>string</code> | If Elasticsearch is protected with basic authentication, this setting provides the password that the Kibana server uses to perform its administrative functions. |
|  [pingTimeout](./kibana-plugin-core-server.elasticsearchconfig.pingtimeout.md) |  | <code>Duration</code> | Timeout after which PING HTTP request will be aborted and retried. |
|  [requestHeadersWhitelist](./kibana-plugin-core-server.elasticsearchconfig.requestheaderswhitelist.md) |  | <code>string[]</code> | List of Kibana client-side headers to send to Elasticsearch when request scoped cluster client is used. If this is an empty array then \*no\* client-side will be sent. |
|  [requestTimeout](./kibana-plugin-core-server.elasticsearchconfig.requesttimeout.md) |  | <code>Duration</code> | Timeout after which HTTP request will be aborted and retried. |
|  [shardTimeout](./kibana-plugin-core-server.elasticsearchconfig.shardtimeout.md) |  | <code>Duration</code> | Timeout for Elasticsearch to wait for responses from shards. Set to 0 to disable. |
|  [sniffInterval](./kibana-plugin-core-server.elasticsearchconfig.sniffinterval.md) |  | <code>false &#124; Duration</code> | Interval to perform a sniff operation and make sure the list of nodes is complete. If <code>false</code> then sniffing is disabled. |
|  [sniffOnConnectionFault](./kibana-plugin-core-server.elasticsearchconfig.sniffonconnectionfault.md) |  | <code>boolean</code> | Specifies whether the client should immediately sniff for a more current list of nodes when a connection dies. |
|  [sniffOnStart](./kibana-plugin-core-server.elasticsearchconfig.sniffonstart.md) |  | <code>boolean</code> | Specifies whether the client should attempt to detect the rest of the cluster when it is first instantiated. |
|  [ssl](./kibana-plugin-core-server.elasticsearchconfig.ssl.md) |  | <code>Pick&lt;SslConfigSchema, Exclude&lt;keyof SslConfigSchema, 'certificateAuthorities' &#124; 'keystore' &#124; 'truststore'&gt;&gt; &amp; {</code><br/><code>        certificateAuthorities?: string[];</code><br/><code>    }</code> | Set of settings configure SSL connection between Kibana and Elasticsearch that are required when <code>xpack.ssl.verification_mode</code> in Elasticsearch is set to either <code>certificate</code> or <code>full</code>. |
|  [username](./kibana-plugin-core-server.elasticsearchconfig.username.md) |  | <code>string</code> | If Elasticsearch is protected with basic authentication, this setting provides the username that the Kibana server uses to perform its administrative functions. |

