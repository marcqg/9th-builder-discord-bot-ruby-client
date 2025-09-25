# NinthBuilderDiscordBotAPIClient::BuildResponse

## Properties

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **success** | **Boolean** |  | [optional] |
| **message** | **String** |  | [optional] |
| **data** | [**BuildResponseData**](BuildResponseData.md) |  | [optional] |

## Example

```ruby
require 'ninth_builder_discord_bot_api_client'

instance = NinthBuilderDiscordBotAPIClient::BuildResponse.new(
  success: true,
  message: Build déclaré avec succès,
  data: null
)
```

