# FastHotel API
FastHotel aims to make the customer able to find the closest hotel to its location. It also orders a taxi to give him a ride to the hotel, and it takes care of the payment process with all its details.
This API provides cheap, fast, and reliable services, which will help the customers to save their time and to give them the best path to the hotel without the need to even know the area or its roads.
# SOA Diagram

![websoa _diagram 2](https://user-images.githubusercontent.com/37571215/50399502-9b106380-0788-11e9-9b06-b0f369fb2bea.png)

# BPMN 2.0 Diagram

![bpmn 2 0_diagramf 3](https://user-images.githubusercontent.com/37571215/50405542-06752800-07bf-11e9-8b77-030904a80de2.png)

# Implementation Details
We developed our service using the RESTful service development paradigm, which is based on the HTTP protocol that is an RPC- based sychronous communication protocol.

#  Composite Service Algorithm According To BPMN 2.0
FastHotelControllerApi

 Example
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
