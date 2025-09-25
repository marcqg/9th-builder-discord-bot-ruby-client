# NinthBuilderDiscordBotAPIClient::GuildsApi

All URIs are relative to *http://localhost:3001*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**guilds_get**](GuildsApi.md#guilds_get) | **GET** /guilds | Get all guilds |


## guilds_get

> <GetGuildsResponse> guilds_get

Get all guilds

Retrieve a list of all Discord guild IDs the bot is connected to

### Examples

```ruby
require 'time'
require 'ninth_builder_discord_bot_api_client'
# setup authorization
NinthBuilderDiscordBotAPIClient.configure do |config|
  # Configure API key authorization: ApiKeyAuth
  config.api_key['Authorization'] = 'YOUR API KEY'
  # Uncomment the following line to set a prefix for the API key, e.g. 'Bearer' (defaults to nil)
  # config.api_key_prefix['Authorization'] = 'Bearer'
end

api_instance = NinthBuilderDiscordBotAPIClient::GuildsApi.new

begin
  # Get all guilds
  result = api_instance.guilds_get
  p result
rescue NinthBuilderDiscordBotAPIClient::ApiError => e
  puts "Error when calling GuildsApi->guilds_get: #{e}"
end
```

#### Using the guilds_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<GetGuildsResponse>, Integer, Hash)> guilds_get_with_http_info

```ruby
begin
  # Get all guilds
  data, status_code, headers = api_instance.guilds_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <GetGuildsResponse>
rescue NinthBuilderDiscordBotAPIClient::ApiError => e
  puts "Error when calling GuildsApi->guilds_get_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**GetGuildsResponse**](GetGuildsResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

