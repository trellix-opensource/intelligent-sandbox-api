# Trellix Intelligent Sandbox (Former: ATD)
The OpenAPI specification for interacting with REST APIs that [Trellix Intelligent Sandbox](https://docs.trellix.com/en/bundle?labelkey=prod-advanced-threat-defense) (former: ATD) offers. <br/>
## How to generate SDKs?

### Setting up the OpenAPI Generator in your environment (one time step)
1. Navigate to: [OpenAPI Generator installation](https://openapi-generator.tech/docs/installation/)
2. Choose the CLI client that suits your need/integrates with your platform better. (**Recommended to use v5.0.1+)**  For more info please visit: https://openapi-generator.tech <br/>
3. The OpenAPI Generator supports many different integrations and use cases, including (but not limited to):
    - Maven Plugin
    - Gradle Plugin
    - Bazel Plugin
    - SBT Plugin
    - Cake Plugin
    - CLI via Homebrew
    - CLI via Docker
    - CLI via npm
    - Generator SaaS<br>
  For details, see [Workflow Integrations](https://openapi-generator.tech/docs/integrations/)

**NOTE:** 
<br/>
In some cases the cli generator might be named as <code>openapi-generator-cli</code> instead of <code>openapi-generator</code>, please be cautious.

### Generating the SDK 
1. Run the following command and make sure you are **running version 5.0+.** [Find the latest version here](https://github.com/OpenAPITools/openapi-generator/releases) <br>
    <code>openapi-generator version</code>
2. For listing out the available languages you can use:<br/>
  <code>openapi-generator list</code><br>
  Alternatively, you can visit: [List of client generators](https://openapi-generator.tech/docs/generators/#client-generators) for list of supported client SDKs.
3. For generating the client in the language of your choice, run the following: <br/>
 <code>openapi-generator generate -i input_file_name.yaml -g a_language_name_from_list -o /path/to/output_folder</code> <br/>
 <br/>
<b>NOTE:</b>
<br/>
 1. If during execution you encounter an error saying "any module/model name" not found, kindly generate the client using the following global property:<br/>
 <code>openapi-generator generate -i file_name.yaml -g a_language_name_from_list -o /path/to/output_folder --global-property skipFormModel=false</code><br/>

## Importing openapi spec in Postman
In order to import the [OpenAPI](openapi.yaml) file in postman, please refer to : [working with openAPI](https://learning.postman.com/docs/integrations/available-integrations/working-with-openAPI/)

## Contributing and Code of conduct
 For Code of conduct and contribution guidelines please refer to [CODE_OF_CONDUCT](CODE_OF_CONDUCT.md) and [CONTRIBUTING](CONTRIBUTING.md) respectively.
 

