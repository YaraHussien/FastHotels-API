# TaxiControllerApi

All URIs are relative to *https://localhost:8080*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getCustomerlocationUsingGET**](TaxiControllerApi.md#getCustomerlocationUsingGET) | **GET** /taxies/taxies-Customer-Location | Get Location of The customer
[**getPathToCustomerUsingGET**](TaxiControllerApi.md#getPathToCustomerUsingGET) | **GET** /taxies/taxies-Direction-OfCustomer | Get Location of The customer


<a name="getCustomerlocationUsingGET"></a>
# **getCustomerlocationUsingGET**
> CustomerModelClass getCustomerlocationUsingGET(customerLocation, id)

Get Location of The customer

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.TaxiControllerApi;


TaxiControllerApi apiInstance = new TaxiControllerApi();
String customerLocation = "32.80045,34.995066"; // String | CustomerLocation
Integer id = 10; // Integer | id
try {
    CustomerModelClass result = apiInstance.getCustomerlocationUsingGET(customerLocation, id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TaxiControllerApi#getCustomerlocationUsingGET");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customerLocation** | **String**| CustomerLocation | [optional] [default to 32.80045,34.995066]
 **id** | **Integer**| id | [optional] [default to 10]

### Return type

[**CustomerModelClass**](CustomerModelClass.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a name="getPathToCustomerUsingGET"></a>
# **getPathToCustomerUsingGET**
> CustomerModelClass getPathToCustomerUsingGET(customerLocation, taxiLocation, id)

Get Location of The customer

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.TaxiControllerApi;


TaxiControllerApi apiInstance = new TaxiControllerApi();
String customerLocation = "32.80045,34.995066"; // String | CustomerLocation
String taxiLocation = "31.783528,35.227093"; // String | TaxiLocation
Integer id = 10; // Integer | id
try {
    CustomerModelClass result = apiInstance.getPathToCustomerUsingGET(customerLocation, taxiLocation, id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TaxiControllerApi#getPathToCustomerUsingGET");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customerLocation** | **String**| CustomerLocation | [optional] [default to 32.80045,34.995066]
 **taxiLocation** | **String**| TaxiLocation | [optional] [default to 31.783528,35.227093]
 **id** | **Integer**| id | [optional] [default to 10]

### Return type

[**CustomerModelClass**](CustomerModelClass.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

