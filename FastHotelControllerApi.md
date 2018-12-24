# FastHotelControllerApi

All URIs are relative to *https://localhost:8080*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addCustomerUsingPOST1**](FastHotelControllerApi.md#addCustomerUsingPOST1) | **POST** /composite/customer | addCustomer
[**findCustomerByNameUsingGET1**](FastHotelControllerApi.md#findCustomerByNameUsingGET1) | **GET** /composite/customer | findCustomerByName
[**getCustomerByIDUsingGET1**](FastHotelControllerApi.md#getCustomerByIDUsingGET1) | **GET** /composite/customer/{id} | getCustomerByID
[**getCustomersUsingGET1**](FastHotelControllerApi.md#getCustomersUsingGET1) | **GET** /composite | customers
[**getDirectioForHotelUsingGET**](FastHotelControllerApi.md#getDirectioForHotelUsingGET) | **GET** /composite/Customer-direction | Get Customer by Location


<a name="addCustomerUsingPOST1"></a>
# **addCustomerUsingPOST1**
> CustomerModelClass addCustomerUsingPOST1(u)

addCustomer

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.FastHotelControllerApi;


FastHotelControllerApi apiInstance = new FastHotelControllerApi();
CustomerModelClass u = new CustomerModelClass(); // CustomerModelClass | u
try {
    CustomerModelClass result = apiInstance.addCustomerUsingPOST1(u);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling FastHotelControllerApi#addCustomerUsingPOST1");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **u** | [**CustomerModelClass**](CustomerModelClass.md)| u |

### Return type

[**CustomerModelClass**](CustomerModelClass.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

<a name="findCustomerByNameUsingGET1"></a>
# **findCustomerByNameUsingGET1**
> String findCustomerByNameUsingGET1(name)

findCustomerByName

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.FastHotelControllerApi;


FastHotelControllerApi apiInstance = new FastHotelControllerApi();
String name = "Yara"; // String | name
try {
    String result = apiInstance.findCustomerByNameUsingGET1(name);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling FastHotelControllerApi#findCustomerByNameUsingGET1");
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

<a name="getCustomerByIDUsingGET1"></a>
# **getCustomerByIDUsingGET1**
> CustomerModelClass getCustomerByIDUsingGET1(id)

getCustomerByID

This operation retrieves a Customer by it&#39;s ID

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.FastHotelControllerApi;


FastHotelControllerApi apiInstance = new FastHotelControllerApi();
Integer id = 56; // Integer | id
try {
    CustomerModelClass result = apiInstance.getCustomerByIDUsingGET1(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling FastHotelControllerApi#getCustomerByIDUsingGET1");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| id |

### Return type

[**CustomerModelClass**](CustomerModelClass.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

<a name="getCustomersUsingGET1"></a>
# **getCustomersUsingGET1**
> List&lt;Object&gt; getCustomersUsingGET1()

customers

This operation retrieves all customers 

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.FastHotelControllerApi;


FastHotelControllerApi apiInstance = new FastHotelControllerApi();
try {
    List<Object> result = apiInstance.getCustomersUsingGET1();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling FastHotelControllerApi#getCustomersUsingGET1");
    e.printStackTrace();
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

**List&lt;Object&gt;**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/xml, application/json

<a name="getDirectioForHotelUsingGET"></a>
# **getDirectioForHotelUsingGET**
> CustomerModelClass getDirectioForHotelUsingGET(id, location, name)

Get Customer by Location

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.FastHotelControllerApi;


FastHotelControllerApi apiInstance = new FastHotelControllerApi();
Integer id = 0; // Integer | id
String location = "31.922428,35.208054"; // String | location
String name = "yara"; // String | name
try {
    CustomerModelClass result = apiInstance.getDirectioForHotelUsingGET(id, location, name);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling FastHotelControllerApi#getDirectioForHotelUsingGET");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **Integer**| id | [optional] [default to 0]
 **location** | **String**| location | [optional] [default to 31.922428,35.208054]
 **name** | **String**| name | [optional] [default to yara]

### Return type

[**CustomerModelClass**](CustomerModelClass.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: */*

