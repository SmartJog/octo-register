# octo-register

Register deployment on octo-spy.

## Role variables

To use octo-register, you need to provide this inventory variable:

* *octo_spy_host*: Complete URL of octo-spy API, example with local api: http://localhost:8080/octo-spy/api

When you call this role in a playbook, you need to specify these variables:

* *project_name*: Name of project in octo-spy, example: "harmony"
* *project_version*: Version of project in octo-spy, example: "v1.0.0"

