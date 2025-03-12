# PMCore/Client\AlipayApi

All URIs are relative to https://api-staging.paomo.fun, except if the operation defines another base path.

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**alipayCreateOrder()**](AlipayApi.md#alipayCreateOrder) | **POST** /Alipay/{appKey}/CreateOrder | 创建订单 - 当面付 |
| [**alipayCreateOrderPagePay()**](AlipayApi.md#alipayCreateOrderPagePay) | **POST** /Alipay/{appKey}/CreateOrderPagePay | 创建订单 - PC支付 |
| [**alipayCreateOrderWapPay()**](AlipayApi.md#alipayCreateOrderWapPay) | **POST** /Alipay/{appKey}/CreateOrderWapPay | 创建订单 - WAP支付 |
| [**alipayOrderDetail()**](AlipayApi.md#alipayOrderDetail) | **GET** /Alipay/{appKey}/OrderDetail | 订单详情 |
| [**alipayOrderRefund()**](AlipayApi.md#alipayOrderRefund) | **POST** /Alipay/{appKey}/OrderRefund | 订单退款 |
| [**alipayReturnPageNotify()**](AlipayApi.md#alipayReturnPageNotify) | **POST** /Alipay/{appKey}/ReturnPageNotify | 支付成功同步通知 |


## `alipayCreateOrder()`

```php
alipayCreateOrder($app_key, $alipay_create_order_request): \PMCore/Client\PMCore/Client/Model\JObjectApiResult
```

创建订单 - 当面付

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: Bearer
$config = PMCore/Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new PMCore/Client\Api\AlipayApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$app_key = 'app_key_example'; // string
$alipay_create_order_request = new \PMCore/Client\PMCore/Client/Model\AlipayCreateOrderRequest(); // \PMCore/Client\PMCore/Client/Model\AlipayCreateOrderRequest

try {
    $result = $apiInstance->alipayCreateOrder($app_key, $alipay_create_order_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AlipayApi->alipayCreateOrder: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **app_key** | **string**|  | |
| **alipay_create_order_request** | [**\PMCore/Client\PMCore/Client/Model\AlipayCreateOrderRequest**](../Model/AlipayCreateOrderRequest.md)|  | [optional] |

### Return type

[**\PMCore/Client\PMCore/Client/Model\JObjectApiResult**](../Model/JObjectApiResult.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: `application/json-patch+json`, `application/json`, `text/json`, `application/*+json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `alipayCreateOrderPagePay()`

```php
alipayCreateOrderPagePay($app_key, $alipay_create_order_page_pay_request): \PMCore/Client\PMCore/Client/Model\JObjectApiResult
```

创建订单 - PC支付

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: Bearer
$config = PMCore/Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new PMCore/Client\Api\AlipayApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$app_key = 'app_key_example'; // string
$alipay_create_order_page_pay_request = new \PMCore/Client\PMCore/Client/Model\AlipayCreateOrderPagePayRequest(); // \PMCore/Client\PMCore/Client/Model\AlipayCreateOrderPagePayRequest

try {
    $result = $apiInstance->alipayCreateOrderPagePay($app_key, $alipay_create_order_page_pay_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AlipayApi->alipayCreateOrderPagePay: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **app_key** | **string**|  | |
| **alipay_create_order_page_pay_request** | [**\PMCore/Client\PMCore/Client/Model\AlipayCreateOrderPagePayRequest**](../Model/AlipayCreateOrderPagePayRequest.md)|  | [optional] |

### Return type

[**\PMCore/Client\PMCore/Client/Model\JObjectApiResult**](../Model/JObjectApiResult.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: `application/json-patch+json`, `application/json`, `text/json`, `application/*+json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `alipayCreateOrderWapPay()`

```php
alipayCreateOrderWapPay($app_key, $alipay_create_order_wap_pay_request): \PMCore/Client\PMCore/Client/Model\JObjectApiResult
```

创建订单 - WAP支付

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: Bearer
$config = PMCore/Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new PMCore/Client\Api\AlipayApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$app_key = 'app_key_example'; // string
$alipay_create_order_wap_pay_request = new \PMCore/Client\PMCore/Client/Model\AlipayCreateOrderWapPayRequest(); // \PMCore/Client\PMCore/Client/Model\AlipayCreateOrderWapPayRequest

try {
    $result = $apiInstance->alipayCreateOrderWapPay($app_key, $alipay_create_order_wap_pay_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AlipayApi->alipayCreateOrderWapPay: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **app_key** | **string**|  | |
| **alipay_create_order_wap_pay_request** | [**\PMCore/Client\PMCore/Client/Model\AlipayCreateOrderWapPayRequest**](../Model/AlipayCreateOrderWapPayRequest.md)|  | [optional] |

### Return type

[**\PMCore/Client\PMCore/Client/Model\JObjectApiResult**](../Model/JObjectApiResult.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: `application/json-patch+json`, `application/json`, `text/json`, `application/*+json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `alipayOrderDetail()`

```php
alipayOrderDetail($app_key, $order_no): \PMCore/Client\PMCore/Client/Model\JObjectApiResult
```

订单详情

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: Bearer
$config = PMCore/Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new PMCore/Client\Api\AlipayApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$app_key = 'app_key_example'; // string
$order_no = 'order_no_example'; // string | 订单号

try {
    $result = $apiInstance->alipayOrderDetail($app_key, $order_no);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AlipayApi->alipayOrderDetail: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **app_key** | **string**|  | |
| **order_no** | **string**| 订单号 | [optional] |

### Return type

[**\PMCore/Client\PMCore/Client/Model\JObjectApiResult**](../Model/JObjectApiResult.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `alipayOrderRefund()`

```php
alipayOrderRefund($app_key, $amount, $order_no): \PMCore/Client\PMCore/Client/Model\JObjectApiResult
```

订单退款

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: Bearer
$config = PMCore/Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new PMCore/Client\Api\AlipayApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$app_key = 'app_key_example'; // string
$amount = 'amount_example'; // string | 退款金额
$order_no = 'order_no_example'; // string | 订单号

try {
    $result = $apiInstance->alipayOrderRefund($app_key, $amount, $order_no);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AlipayApi->alipayOrderRefund: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **app_key** | **string**|  | |
| **amount** | **string**| 退款金额 | [optional] |
| **order_no** | **string**| 订单号 | [optional] |

### Return type

[**\PMCore/Client\PMCore/Client/Model\JObjectApiResult**](../Model/JObjectApiResult.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)

## `alipayReturnPageNotify()`

```php
alipayReturnPageNotify($app_key, $return_page_notify_request): \PMCore/Client\PMCore/Client/Model\JObjectApiResult
```

支付成功同步通知

### Example

```php
<?php
require_once(__DIR__ . '/vendor/autoload.php');


// Configure Bearer authorization: Bearer
$config = PMCore/Client\Configuration::getDefaultConfiguration()->setAccessToken('YOUR_ACCESS_TOKEN');


$apiInstance = new PMCore/Client\Api\AlipayApi(
    // If you want use custom http client, pass your client which implements `GuzzleHttp\ClientInterface`.
    // This is optional, `GuzzleHttp\Client` will be used as default.
    new GuzzleHttp\Client(),
    $config
);
$app_key = 'app_key_example'; // string
$return_page_notify_request = new \PMCore/Client\PMCore/Client/Model\ReturnPageNotifyRequest(); // \PMCore/Client\PMCore/Client/Model\ReturnPageNotifyRequest

try {
    $result = $apiInstance->alipayReturnPageNotify($app_key, $return_page_notify_request);
    print_r($result);
} catch (Exception $e) {
    echo 'Exception when calling AlipayApi->alipayReturnPageNotify: ', $e->getMessage(), PHP_EOL;
}
```

### Parameters

| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **app_key** | **string**|  | |
| **return_page_notify_request** | [**\PMCore/Client\PMCore/Client/Model\ReturnPageNotifyRequest**](../Model/ReturnPageNotifyRequest.md)|  | [optional] |

### Return type

[**\PMCore/Client\PMCore/Client/Model\JObjectApiResult**](../Model/JObjectApiResult.md)

### Authorization

[Bearer](../../README.md#Bearer)

### HTTP request headers

- **Content-Type**: `application/json-patch+json`, `application/json`, `text/json`, `application/*+json`
- **Accept**: `application/json`

[[Back to top]](#) [[Back to API list]](../../README.md#endpoints)
[[Back to Model list]](../../README.md#models)
[[Back to README]](../../README.md)
