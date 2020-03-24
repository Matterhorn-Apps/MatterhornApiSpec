# MatterhornApiSpec
This repository contains versioned OpenAPI specs for [MatterhornApiService](https://github.com/Matterhorn-Apps/MatterhornApiService). These specs are defined using OpenAPI v3.

This repository is included as a submodule by other repositories and the specs are used to generate server and client code for hosting and consuming instances of the Matterhorn API.

## Specs
Versioned API specs are stored in the `specs` directory at the root of the repository. Each spec is named according to the pattern `x.y.z.yaml` where `x.y.z` corresponds to the version of the defined spec. Version numbers should be chosen according to [semantic versioning rules](https://semver.org/).

### Creating a new version of the spec
In most cases, making a change to the spec means creating a new version. (If you are changing a spec definition without bumping the version number, you should have no existing consumers for the spec, or be very sure that you know what you are doing.)

VSCode tasks are defined to start or stop a Docker container hosting an instance of [Swagger-Editor](https://swagger.io/tools/swagger-editor/). This tool can be used to view and edit an OpenAPI spec, and to save a new copy of the spec to disk.