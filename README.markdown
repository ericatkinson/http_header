# HTTP Header #

Set the HTTP Headers for your template.

## Parameters

* status - input an HTTP Status code
* location - set a location for redirection
* content_type - set a Content-Type header
* terminate - set to "yes" to prevent any other output from the template

## Examples

Do a 301 redirect
	{exp:http_header status="302" location="{path=site/something}" terminate="yes"}

Set a 404 Status header
	{exp:http_header status="404"}

Set the Content-Type header to application/json
	{exp:http_header content_type="application/json"}