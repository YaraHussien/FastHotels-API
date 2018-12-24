# PayBalControllerApi

All URIs are relative to *https://localhost:8080*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getDetailsUsingGET**](PayBalControllerApi.md#getDetailsUsingGET) | **GET** /paybal/Get-Customer-Payment-Details | getDetails


<a name="getDetailsUsingGET"></a>
# **getDetailsUsingGET**
> String getDetailsUsingGET(name)

getDetails

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.PayBalControllerApi;


PayBalControllerApi apiInstance = new PayBalControllerApi();
String name = "Yara"; // String | name
try {
    String result = apiInstance.getDetailsUsingGET(name);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PayBalControllerApi#getDetailsUsingGET");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **String**| name | [optional] [default to Yara]

### Return type

**String**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

