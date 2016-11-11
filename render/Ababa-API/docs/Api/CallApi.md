# Swagger\Client\CallApi

All URIs are relative to *http://www.ababa.io/websvr/v1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getCallByName**](CallApi.md#getCallByName) | **GET** /call/searchCallByFileName | Returns a specific call record referenced by the filename / filetitle given
[**searchCallByCallID**](CallApi.md#searchCallByCallID) | **GET** /call/searchCallByCallID | Returns a specific call record referenced by the ID given


# **getCallByName**
> \Swagger\Client\Model\CallResponseFilename getCallByName($filename)

Returns a specific call record referenced by the filename / filetitle given

Returns a list of calls of the given matching criteria

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CallApi();
$filename = "filename_example"; // string | Search Call by filename

try {
    $result = $api_instance->getCallByName($filename);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CallApi->getCallByName: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **filename** | **string**| Search Call by filename |

### Return type

[**\Swagger\Client\Model\CallResponseFilename**](../Model/CallResponseFilename.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

# **searchCallByCallID**
> \Swagger\Client\Model\CallResponse searchCallByCallID($id)

Returns a specific call record referenced by the ID given

Returns a list of calls of the given matching criteria

### Example
```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');

$api_instance = new Swagger\Client\Api\CallApi();
$id = 56; // int | Identification FileID for the end point record to be returned

try {
    $result = $api_instance->searchCallByCallID($id);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling CallApi->searchCallByCallID: ', $e->getMessage(), PHP_EOL;
}
?>
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **int**| Identification FileID for the end point record to be returned |

### Return type

[**\Swagger\Client\Model\CallResponse**](../Model/CallResponse.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

[[Back to top]](#) [[Back to API list]](../../README.md#documentation-for-api-endpoints) [[Back to Model list]](../../README.md#documentation-for-models) [[Back to README]](../../README.md)

