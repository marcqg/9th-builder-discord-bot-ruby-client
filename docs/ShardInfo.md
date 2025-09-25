# NinthBuilderDiscordBotAPIClient::ShardInfo

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **Float** | Shard ID | [optional] |
| **ready** | **Boolean** | Whether the shard is ready | [optional] |
| **error** | **Boolean** | Whether the shard has an error | [optional] |
| **uptime_secs** | **Float** | Uptime in seconds | [optional] |

## Example

```ruby
require 'ninth_builder_discord_bot_api_client'

instance = NinthBuilderDiscordBotAPIClient::ShardInfo.new(
  id: 0,
  ready: true,
  error: false,
  uptime_secs: 3600
)
```

