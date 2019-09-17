# cd-manifests
Single Source of Truth (Manifest files) for CD settings of argo-cd

NOTE: `Application` means a unit of an argo-cd deployment setting here. It's a kind of CRD defined in the argo-cd.

# Contents
* `/*-app.yaml`
  * `Application` for `Application`s which manage user applications
* `/*-sys.yaml`
  * `Application` for `Application`s which manage system applications
    * **NOTE: Contains a hacky solution, which uses external values files. Until manual sync from UI or CLI, won't be synced**

<!-- -->

* `/dev-*.yaml`
  * Files for the development env
* `/prd-*.yaml`
  * Files for the production env

<!-- -->

* `/*/app/*.yaml`
  * `Application`s which manage user applications
* `/*/sys/*.yaml`
  * `Application`s which manage system applications

<!-- -->

* `/dev/*/*.yaml`
  * Files for the development env
* `/prd/*/*.yaml`
  * Files for the production env
