# app-operator
- operator-sdk add controller --api-version=app.example.com/v1beta1 --kind=AppService
- operator-sdk add api --api-version=app.example.com/v1beta1 --kind=AppService
- operator-courier push deploy/olm-catalog/app-operator/ "$QUAY_NAMESPACE" "$PACKAGE_NAME" "$PACKAGE_VERSION" "$QUAY_TOKEN"