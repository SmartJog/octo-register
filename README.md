# octo-register

Register deployment on octo-spy.

## Usage

There are two usages of this roles, defined by variables *step*, possibles steps are:
* "start": Register deployment.
* "end": Delete progress of registered deployment. Call it only if step init has been called and variable *project_progress* has been set to true.

## Role variables

To use octo-register, you need to provide this inventory variable:

* *octo_spy_host*: Complete URL of octo-spy API, example with local api: http://localhost:8080/octo-spy/api
* *octo_username*: Username for the octo-spy API
* *octo_password*: Password for the octo-spy API

When you call this role in a playbook, you need to specify these variables:

* *project_name*: Name of project in octo-spy, example: "harmony"
* *project_version*: Version of project in octo-spy, example: "v1.0.0"
* *project_environment*: Environment of project in octo-spy, valid values: "Development", "QA", "Integration", "Pre-production" and "Production"
  Project environment is optional, the default value is "Development".
* *project_client*: Client of project in octo-spy.
  Project client is optional, the default value is "Internal".
* *project_progress*: Set progress of deployment, the default value is true.
