# NinthBuilderDiscordBotAPIClient::ShardsApi

All URIs are relative to *http://localhost:3001*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**shards_get**](ShardsApi.md#shards_get) | **GET** /shards | Get shard information |
| [**shards_presence_put**](ShardsApi.md#shards_presence_put) | **PUT** /shards/presence | Set shard presences |


## shards_get

> <GetShardsResponse> shards_get

Get shard information

Retrieve information about all shards including status and statistics

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

api_instance = NinthBuilderDiscordBotAPIClient::ShardsApi.new

begin
  # Get shard information
  result = api_instance.shards_get
  p result
rescue NinthBuilderDiscordBotAPIClient::ApiError => e
  puts "Error when calling ShardsApi->shards_get: #{e}"
end
```

#### Using the shards_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<GetShardsResponse>, Integer, Hash)> shards_get_with_http_info

```ruby
begin
  # Get shard information
  data, status_code, headers = api_instance.shards_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <GetShardsResponse>
rescue NinthBuilderDiscordBotAPIClient::ApiError => e
  puts "Error when calling ShardsApi->shards_get_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**GetShardsResponse**](GetShardsResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## shards_presence_put

> shards_presence_put(set_shard_presences_request)

Set shard presences

Update the presence/activity status of all shards

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

api_instance = NinthBuilderDiscordBotAPIClient::ShardsApi.new
set_shard_presences_request = NinthBuilderDiscordBotAPIClient::SetShardPresencesRequest.new({type: 'Playing', name: 'with Discord.js'}) # SetShardPresencesRequest | 

begin
  # Set shard presences
  api_instance.shards_presence_put(set_shard_presences_request)
rescue NinthBuilderDiscordBotAPIClient::ApiError => e
  puts "Error when calling ShardsApi->shards_presence_put: #{e}"
end
```

#### Using the shards_presence_put_with_http_info variant

This returns an Array which contains the response data (`nil` in this case), status code and headers.

> <Array(nil, Integer, Hash)> shards_presence_put_with_http_info(set_shard_presences_request)

```ruby
begin
  # Set shard presences
  data, status_code, headers = api_instance.shards_presence_put_with_http_info(set_shard_presences_request)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => nil
rescue NinthBuilderDiscordBotAPIClient::ApiError => e
  puts "Error when calling ShardsApi->shards_presence_put_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **set_shard_presences_request** | [**SetShardPresencesRequest**](SetShardPresencesRequest.md) |  |  |

### Return type

nil (empty response body)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

