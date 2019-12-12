# app-operator
- operator-sdk add controller --api-version=app.example.com/v1beta1 --kind=AppService
- operator-sdk add api --api-version=app.example.com/v1beta1 --kind=AppService
- operator-courier push deploy/olm-catalog/app-operator/ "$QUAY_NAMESPACE" "$PACKAGE_NAME" "$PACKAGE_VERSION" "$QUAY_TOKEN"

# How to have a Cluster scoped CRD

- https://github.com/operator-framework/operator-sdk/blob/master/doc/operator-scope.md
- https://github.com/operator-framework/getting-started