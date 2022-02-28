# openapi_client.UsersApi

All URIs are relative to *http://localhost*

Method | HTTP request | Description
------------- | ------------- | -------------
[**active_users_active_users_get**](UsersApi.md#active_users_active_users_get) | **GET** /activeUsers | Print active users
[**logout_logout_post**](UsersApi.md#logout_logout_post) | **POST** /logout | LogOut
[**put_login_post**](UsersApi.md#put_login_post) | **POST** /login | Enter your login
[**put_register_post**](UsersApi.md#put_register_post) | **POST** /register | Register


# **active_users_active_users_get**
> bool, date, datetime, dict, float, int, list, str, none_type active_users_active_users_get()

Print active users

### Example

```python
import time
import openapi_client
from openapi_client.api import users_api
from pprint import pprint
# Defining the host is optional and defaults to http://localhost
# See configuration.py for a list of all supported configuration parameters.
configuration = openapi_client.Configuration(
    host = "http://localhost"
)


# Enter a context with an instance of the API client
with openapi_client.ApiClient() as api_client:
    # Create an instance of the API class
    api_instance = users_api.UsersApi(api_client)

    # example, this endpoint has no required or optional parameters
    try:
        # Print active users
        api_response = api_instance.active_users_active_users_get()
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling UsersApi->active_users_active_users_get: %s\n" % e)
```


### Parameters
This endpoint does not need any parameter.

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

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **logout_logout_post**
> bool, date, datetime, dict, float, int, list, str, none_type logout_logout_post(user_registration)

LogOut

### Example

```python
import time
import openapi_client
from openapi_client.api import users_api
from openapi_client.model.user_registration import UserRegistration
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
    api_instance = users_api.UsersApi(api_client)
    user_registration = UserRegistration(
        login="login_example",
        password="password_example",
    ) # UserRegistration | 

    # example passing only required values which don't have defaults set
    try:
        # LogOut
        api_response = api_instance.logout_logout_post(user_registration)
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling UsersApi->logout_logout_post: %s\n" % e)
```


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_registration** | [**UserRegistration**](UserRegistration.md)|  |

### Return type

**bool, date, datetime, dict, float, int, list, str, none_type**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **put_login_post**
> bool, date, datetime, dict, float, int, list, str, none_type put_login_post(user_registration)

Enter your login

### Example

```python
import time
import openapi_client
from openapi_client.api import users_api
from openapi_client.model.user_registration import UserRegistration
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
    api_instance = users_api.UsersApi(api_client)
    user_registration = UserRegistration(
        login="login_example",
        password="password_example",
    ) # UserRegistration | 

    # example passing only required values which don't have defaults set
    try:
        # Enter your login
        api_response = api_instance.put_login_post(user_registration)
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling UsersApi->put_login_post: %s\n" % e)
```


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_registration** | [**UserRegistration**](UserRegistration.md)|  |

### Return type

**bool, date, datetime, dict, float, int, list, str, none_type**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

# **put_register_post**
> bool, date, datetime, dict, float, int, list, str, none_type put_register_post(user_registration)

Register

### Example

```python
import time
import openapi_client
from openapi_client.api import users_api
from openapi_client.model.user_registration import UserRegistration
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
    api_instance = users_api.UsersApi(api_client)
    user_registration = UserRegistration(
        login="login_example",
        password="password_example",
    ) # UserRegistration | 

    # example passing only required values which don't have defaults set
    try:
        # Register
        api_response = api_instance.put_register_post(user_registration)
        pprint(api_response)
    except openapi_client.ApiException as e:
        print("Exception when calling UsersApi->put_register_post: %s\n" % e)
```


### Parameters

Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **user_registration** | [**UserRegistration**](UserRegistration.md)|  |

### Return type

**bool, date, datetime, dict, float, int, list, str, none_type**

### Authorization

No authorization required

### HTTP request headers

 - **Content-Type**: application/json
 - **Accept**: application/json


### HTTP response details
| Status code | Description | Response headers |
|-------------|-------------|------------------|
**201** | Successful Response |  -  |
**422** | Validation Error |  -  |

[[Back to top]](#) [[Back to API list]](../README.md#documentation-for-api-endpoints) [[Back to Model list]](../README.md#documentation-for-models) [[Back to README]](../README.md)

