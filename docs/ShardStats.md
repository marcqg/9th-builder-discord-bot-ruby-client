# NinthBuilderDiscordBotAPIClient::ShardStats

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **shard_count** | **Float** | Total number of shards | [optional] |
| **uptime_secs** | **Float** | Manager uptime in seconds | [optional] |

## Example

```ruby
require 'ninth_builder_discord_bot_api_client'

instance = NinthBuilderDiscordBotAPIClient::ShardStats.new(
  shard_count: 2,
  uptime_secs: 7200
)
```

