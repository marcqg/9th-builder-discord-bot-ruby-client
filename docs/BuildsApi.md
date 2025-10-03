# NinthBuilderDiscordBotAPIClient::BuildsApi

All URIs are relative to *http://localhost:3001*

| Method | HTTP request | Description |
| ------ | ------------ | ----------- |
| [**builds_post**](BuildsApi.md#builds_post) | **POST** /builds | Declare a new build |


## builds_post

> <BuildResponse> builds_post(build_declaration)

Declare a new build

Declare a new build with URL, message, and filename

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

api_instance = NinthBuilderDiscordBotAPIClient::BuildsApi.new
build_declaration = NinthBuilderDiscordBotAPIClient::BuildDeclaration.new({url: 'https://example.com/builds/my-build.zip', message: 'New feature implementation', filename: 'my-build-v1.0.0.zip'}) # BuildDeclaration | 

begin
  # Declare a new build
  result = api_instance.builds_post(build_declaration)
  p result
rescue NinthBuilderDiscordBotAPIClient::ApiError => e
  puts "Error when calling BuildsApi->builds_post: #{e}"
end
```

#### Using the builds_post_with_http_info variant

This returns an Array which contains the response data, status code and headers.

> <Array(<BuildResponse>, Integer, Hash)> builds_post_with_http_info(build_declaration)

```ruby
begin
  # Declare a new build
  data, status_code, headers = api_instance.builds_post_with_http_info(build_declaration)
  p status_code # => 2xx
  p headers # => { ... }
  p data # => <BuildResponse>
rescue NinthBuilderDiscordBotAPIClient::ApiError => e
  puts "Error when calling BuildsApi->builds_post_with_http_info: #{e}"
end
```

### Parameters

| Name | Type | Description | Notes |
| ---- | ---- | ----------- | ----- |
| **build_declaration** | [**BuildDeclaration**](BuildDeclaration.md) |  |  |

### Return type

[**BuildResponse**](BuildResponse.md)

### Authorization

[ApiKeyAuth](../README.md#ApiKeyAuth)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

