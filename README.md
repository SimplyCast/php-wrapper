<h1>SimplyCast PHP Wrapper</h1>
	
<h2>Description</h2>
	
<p>The SimplyCast PHP Wrapper helps facilitate integration with the SimplyCast
API. It performs authentication and serialization for many of the resources
in the API and includes some additional helper functionality beyond what the
API provides.<p>
	
<h2>Usage</h2> 
	
<p>Currently, the PHP wrapper is contained in the single included file, 
SimplyCastAPI.php. The API wrapper makes use of namespaces (under 
SimplyCast). To use it give your API keys as a contstructor to the 
main \SimplyCast\API class. Then, you make calls to the helper functions by
calling $api->resourceSubcategory->apiFunction. Example:</p>

```php
$api = new \SimplyCast\API('<publickey>', '<secretkey>');
	
$api->contactManager->getContacts();
$api->simplyCast360->getProject(<project id>);
```
	
<p>Returned responses from the API functions are direct decoded JSON, so the 
array structures returned will mirror the JSON response examples in the API
reference documentation.</p>
	

<h2>Licensing</h2>
	
<p>This software is distributed under the MIT licence. Please see the attached 
file called LICENCE.txt.</p>
