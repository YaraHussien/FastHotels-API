# CustomerControllerApi

All URIs are relative to *https://localhost:8080*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addCustomerUsingPOST**](CustomerControllerApi.md#addCustomerUsingPOST) | **POST** /customer/customer | addCustomer
[**findCustomerByNameUsingGET**](CustomerControllerApi.md#findCustomerByNameUsingGET) | **GET** /customer/customer | findCustomerByName
[**getCustomerByIDUsingGET**](CustomerControllerApi.md#getCustomerByIDUsingGET) | **GET** /customer/customer/{id} | getCustomerByID
[**getCustomersUsingGET**](CustomerControllerApi.md#getCustomersUsingGET) | **GET** /customer | customers


<a name="addCustomerUsingPOST"></a>
# **addCustomerUsingPOST**
> CustomerModelClass addCustomerUsingPOST(c)

addCustomer

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.CustomerControllerApi;


CustomerControllerApi apiInstance = new CustomerControllerApi();
CustomerModelClass c = new CustomerModelClass(); // CustomerModelClass | c
try {
    CustomerModelClass result = apiInstance.addCustomerUsingPOST(c);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerControllerApi#addCustomerUsingPOST");
    e.printStackTrace();
}
```

### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **c** | [**CustomerModelClass**](CustomerModelClass.md)| c |

### Return type

[**CustomerModelClass**](CustomerModelClass.md)

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: */*

<a name="findCustomerByNameUsingGET"></a>
# **findCustomerByNameUsingGET**
> String findCustomerByNameUsingGET(name)

findCustomerByName

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.CustomerControllerApi;


CustomerControllerApi apiInstance = new CustomerControllerApi();
String name = "Yara"; // String | name
try {
    String result = apiInstance.findCustomerByNameUsingGET(name);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerControllerApi#findCustomerByNameUsingGET");
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

<a name="getCustomerByIDUsingGET"></a>
# **getCustomerByIDUsingGET**
> CustomerModelClass getCustomerByIDUsingGET(id)

getCustomerByID

This operation retrieves a Customer by it&#39;s ID

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.CustomerControllerApi;


CustomerControllerApi apiInstance = new CustomerControllerApi();
Integer id = 56; // Integer | id
try {
    CustomerModelClass result = apiInstance.getCustomerByIDUsingGET(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerControllerApi#getCustomerByIDUsingGET");
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

<a name="getCustomersUsingGET"></a>
# **getCustomersUsingGET**
> List&lt;Object&gt; getCustomersUsingGET()

customers

This operation retrieves all customers 

### Example
```java
// Import classes:
//import io.swagger.client.ApiException;
//import io.swagger.client.api.CustomerControllerApi;


CustomerControllerApi apiInstance = new CustomerControllerApi();
try {
    List<Object> result = apiInstance.getCustomersUsingGET();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerControllerApi#getCustomersUsingGET");
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

