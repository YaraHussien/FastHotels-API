# HotelControllerApi

All URIs are relative to *https://localhost:8080*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getHotelsUsingGET**](HotelControllerApi.md#getHotelsUsingGET) | **GET** /hotels | getHotels


<a name="getHotelsUsingGET"></a>
# **getHotelsUsingGET**
> List&lt;HotelModelClass&gt; getHotelsUsingGET()

getHotels

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.HotelControllerApi;


HotelControllerApi apiInstance = new HotelControllerApi();
try {
    List<HotelModelClass> result = apiInstance.getHotelsUsingGET();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling HotelControllerApi#getHotelsUsingGET");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**List&lt;HotelModelClass&gt;**](HotelModelClass.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

