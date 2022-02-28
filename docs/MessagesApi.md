# openapi_client.MessagesApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**get_get_name_sender_get**](MessagesApi.md#get_get_name_sender_get) | **GET** /get/{name}/{sender} | Receive messages
[**get_new_get_new_name_sender_get**](MessagesApi.md#get_new_get_new_name_sender_get) | **GET** /getNew/{name}/{sender} | Get number and content of new messages
[**marked_as_read_marked_as_read_name_sender_put**](MessagesApi.md#marked_as_read_marked_as_read_name_sender_put) | **PUT** /markedAsRead/{name}/{sender} | Mark as read
[**post_all_send_all_post**](MessagesApi.md#post_all_send_all_post) | **POST** /sendAll | Send message to All
[**post_send_sender_username_receiver_username_message_post**](MessagesApi.md#post_send_sender_username_receiver_username_message_post) | **POST** /send/{sender_username}/{receiver_username}/{message} | Send message


# **get_get_name_sender_get**
> bool, date, datetime, dict, float, int, list, str, none_type get_get_name_sender_get(name, sender)

Receive messages

### Example

```python
import time
import openapi_client
from openapi_client.api import messages_api
from openapi_client.model.http_validation_error import HTTPValidationError
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = messages_api.MessagesApi(api_client)
    name = "name_example" # str | 
    sender = "sender_example" # str | 

    # example passing only required values which don't have defaults set
    try:
        # Receive messages
        api_response = api_instance.get_get_name_sender_get(name, sender)
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling MessagesApi->get_get_name_sender_get: %s\n" % e)
```


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  |
 **sender** | **str**|  |

### Return type

**bool, date, datetime, dict, float, int, list, str, none_type**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **get_new_get_new_name_sender_get**
> bool, date, datetime, dict, float, int, list, str, none_type get_new_get_new_name_sender_get(name, sender)

Get number and content of new messages

### Example

```python
import time
import openapi_client
from openapi_client.api import messages_api
from openapi_client.model.http_validation_error import HTTPValidationError
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = messages_api.MessagesApi(api_client)
    name = "name_example" # str | 
    sender = "sender_example" # str | 

    # example passing only required values which don't have defaults set
    try:
        # Get number and content of new messages
        api_response = api_instance.get_new_get_new_name_sender_get(name, sender)
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling MessagesApi->get_new_get_new_name_sender_get: %s\n" % e)
```


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  |
 **sender** | **str**|  |

### Return type

**bool, date, datetime, dict, float, int, list, str, none_type**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **marked_as_read_marked_as_read_name_sender_put**
> bool, date, datetime, dict, float, int, list, str, none_type marked_as_read_marked_as_read_name_sender_put(name, sender)

Mark as read

### Example

```python
import time
import openapi_client
from openapi_client.api import messages_api
from openapi_client.model.http_validation_error import HTTPValidationError
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = messages_api.MessagesApi(api_client)
    name = "name_example" # str | 
    sender = "sender_example" # str | 

    # example passing only required values which don't have defaults set
    try:
        # Mark as read
        api_response = api_instance.marked_as_read_marked_as_read_name_sender_put(name, sender)
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling MessagesApi->marked_as_read_marked_as_read_name_sender_put: %s\n" % e)
```


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **name** | **str**|  |
 **sender** | **str**|  |

### Return type

**bool, date, datetime, dict, float, int, list, str, none_type**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**200** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_all_send_all_post**
> bool, date, datetime, dict, float, int, list, str, none_type post_all_send_all_post(sender_username, receiver_username, message)

Send message to All

### Example

```python
import time
import openapi_client
from openapi_client.api import messages_api
from openapi_client.model.http_validation_error import HTTPValidationError
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = messages_api.MessagesApi(api_client)
    sender_username = "sender_username_example" # str | 
    receiver_username = "receiver_username_example" # str | 
    message = "message_example" # str | 

    # example passing only required values which don't have defaults set
    try:
        # Send message to All
        api_response = api_instance.post_all_send_all_post(sender_username, receiver_username, message)
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling MessagesApi->post_all_send_all_post: %s\n" % e)
```


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sender_username** | **str**|  |
 **receiver_username** | **str**|  |
 **message** | **str**|  |

### Return type

**bool, date, datetime, dict, float, int, list, str, none_type**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **post_send_sender_username_receiver_username_message_post**
> bool, date, datetime, dict, float, int, list, str, none_type post_send_sender_username_receiver_username_message_post(sender_username, receiver_username, message)

Send message

### Example

```python
import time
import openapi_client
from openapi_client.api import messages_api
from openapi_client.model.http_validation_error import HTTPValidationError
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = messages_api.MessagesApi(api_client)
    sender_username = "sender_username_example" # str | 
    receiver_username = "receiver_username_example" # str | 
    message = "message_example" # str | 

    # example passing only required values which don't have defaults set
    try:
        # Send message
        api_response = api_instance.post_send_sender_username_receiver_username_message_post(sender_username, receiver_username, message)
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling MessagesApi->post_send_sender_username_receiver_username_message_post: %s\n" % e)
```


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **sender_username** | **str**|  |
 **receiver_username** | **str**|  |
 **message** | **str**|  |

### Return type

**bool, date, datetime, dict, float, int, list, str, none_type**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

