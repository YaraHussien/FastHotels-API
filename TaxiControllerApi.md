# TaxiControllerApi

All URIs are relative to *https://localhost:8080*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getDirectioForHotelUsingGET1**](TaxiControllerApi.md#getDirectioForHotelUsingGET1) | **GET** /taxies/PickUp-Customer | Get Direction of The customer


<a name="getDirectioForHotelUsingGET1"></a>
# **getDirectioForHotelUsingGET1**
> CustomerModelClass getDirectioForHotelUsingGET1(customerLocation, taxiLocation, id)

Get Direction of The customer

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.TaxiControllerApi;


TaxiControllerApi apiInstance = new TaxiControllerApi();
String customerLocation = "31.922428,35.208054"; // String | CustomerLocation
String taxiLocation = "31.9224179,35.2277767"; // String | TaxiLocation
Integer id = 0; // Integer | id
try {
    CustomerModelClass result = apiInstance.getDirectioForHotelUsingGET1(customerLocation, taxiLocation, id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TaxiControllerApi#getDirectioForHotelUsingGET1");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customerLocation** | **String**| CustomerLocation | [optional] [default to 31.922428,35.208054]
 **taxiLocation** | **String**| TaxiLocation | [optional] [default to 31.9224179,35.2277767]
 **id** | **Integer**| id | [optional] [default to 0]

### Return type

[**CustomerModelClass**](CustomerModelClass.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

