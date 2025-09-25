# NinthBuilderDiscordBotAPIClient::SetShardPresencesRequest

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **type** | **String** | Activity type |  |
| **name** | **String** | Activity name |  |
| **url** | **String** | Stream URL (only for Streaming type) | [optional] |

## Example

```ruby
require 'ninth_builder_discord_bot_api_client'

instance = NinthBuilderDiscordBotAPIClient::SetShardPresencesRequest.new(
  type: Playing,
  name: with Discord.js,
  url: https://twitch.tv/example
)
```

