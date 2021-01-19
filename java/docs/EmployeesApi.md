# EmployeesApi

All URIs are relative to *https://virtserver.swaggerhub.com/DMI_Software/DMI_Software_Employees/1*

Method | HTTP request | Description
------------- | ------------- | -------------
[**employeesIdGet**](EmployeesApi.md#employeesIdGet) | **GET** /employees/{id} | Get the dmi employees information


<a name="employeesIdGet"></a>
# **employeesIdGet**
> ResponseCode employeesIdGet(id, authorization)

Get the dmi employees information

Get employees info

### Example
```java
// Import classes:
//import io.swagger.client.ApiClient;
//import io.swagger.client.ApiException;
//import io.swagger.client.Configuration;
//import io.swagger.client.auth.*;
//import io.swagger.client.api.EmployeesApi;

ApiClient defaultClient = Configuration.getDefaultApiClient();

// Configure API key authorization: Bearer
ApiKeyAuth Bearer = (ApiKeyAuth) defaultClient.getAuthentication("Bearer");
Bearer.setApiKey("YOUR API KEY");
// Uncomment the following line to set a prefix for the API key, e.g. "Token" (defaults to null)
//Bearer.setApiKeyPrefix("Token");

EmployeesApi apiInstance = new EmployeesApi();
Integer id = 56; // Integer | employee id
String authorization = "authorization_example"; // String | token to be passed as a header
try {
    ResponseCode result = apiInstance.employeesIdGet(id, authorization);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EmployeesApi#employeesIdGet");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| employee id |
 **authorization** | **String**| token to be passed as a header | [optional]

### Return type

[**ResponseCode**](ResponseCode.md)

### Authorization

[Bearer](../README.md#Bearer)

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: Not defined

