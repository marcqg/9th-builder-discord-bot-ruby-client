# NinthBuilderDiscordBotAPIClient::GeneralApi

All URIs are relative to *http://localhost:3001*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**root_get**](GeneralApi.md#root_get) | **GET** / | Get API information |


## root_get

> <ApiInfo> root_get

Get API information

Returns basic information about the API

### Examples

```ruby
require 'time'
require 'ninth_builder_discord_bot_api_client'

api_instance = NinthBuilderDiscordBotAPIClient::GeneralApi.new

begin
  # Get API information
  result = api_instance.root_get
  p result
rescue NinthBuilderDiscordBotAPIClient::ApiError => e
  puts "Error when calling GeneralApi->root_get: #{e}"
end
```

#### Using the root_get_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<ApiInfo>, Integer, Hash)> root_get_with_http_info

```ruby
begin
  # Get API information
  data, status_code, headers = api_instance.root_get_with_http_info
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <ApiInfo>
rescue NinthBuilderDiscordBotAPIClient::ApiError => e
  puts "Error when calling GeneralApi->root_get_with_http_info: #{e}"
end
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**ApiInfo**](ApiInfo.md)

### Authorization

No authorization required

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

