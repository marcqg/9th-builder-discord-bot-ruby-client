# NinthBuilderDiscordBotAPIClient::BuildDeclaration

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **url** | **String** | URL of the build artifact |  |
| **message** | **String** | Build message or description |  |
| **filename** | **String** | Name of the build file |  |

## Example

```ruby
require 'ninth_builder_discord_bot_api_client'

instance = NinthBuilderDiscordBotAPIClient::BuildDeclaration.new(
  url: https://example.com/builds/my-build.zip,
  message: New feature implementation,
  filename: my-build-v1.0.1.zip
)
```

