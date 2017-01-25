# SwaggerMFPAdapterGenerator
Generate MobileFirst Foundation adapters for a REST backend

## Steps to run the MFP Adapter Generator

* Go to  ```mfp-adapters-swagger-codegen``` directory.
* Run ```mvn install```
* In adpater-generator/Config.json customise the adapter properties like adapter name etc.
* Add the swagger json of the endpoint.
* Go to ```adapter-generator``` directory.
* Run the generator using ```mvn io.swagger:swagger-codegen-maven-plugin:2.1.6:generate```

The generated adapter file will be available in ../generatedAdapter folder.

The adapter binary needs to be built using ```mfpdev adapter build```.

** Conditions Apply
* Currently working on for GET requests.