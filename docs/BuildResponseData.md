# NinthBuilderDiscordBotAPIClient::BuildResponseData

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **id** | **Float** |  | [optional] |
| **url** | **String** |  | [optional] |
| **message** | **String** |  | [optional] |
| **filename** | **String** |  | [optional] |
| **created_at** | **Time** |  | [optional] |

## Example

```ruby
require 'ninth_builder_discord_bot_api_client'

instance = NinthBuilderDiscordBotAPIClient::BuildResponseData.new(
  id: 1672531200000,
  url: https://example.com/builds/my-build.zip,
  message: New feature implementation,
  filename: my-build-v1.0.0.zip,
  created_at: 2023-01-01T00:00Z
)
```

