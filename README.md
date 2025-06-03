# Demo of CEL admission controllers

https://kubernetes.io/docs/reference/access-authn-authz/validating-admission-policy/#validation-expression





- 'object' - The object from the incoming request. The value is null for DELETE requests.
- 'oldObject' - The existing object. The value is null for CREATE requests.
- 'request' - Attributes of the admission request.
- 'params' - Parameter resource referred to by the policy binding being evaluated. The value is null if ParamKind is not specified.
- namespaceObject - The namespace, as a Kubernetes resource, that the incoming object belongs to. The value is null if the incoming object is cluster-scoped.
- authorizer - A CEL Authorizer. May be used to perform authorization checks for the principal (authenticated user) of the request. See AuthzSelectors and Authz in the Kubernetes CEL library documentation for more details.
- authorizer.requestResource - A shortcut for an authorization check configured with the request resource (group, resource, (subresource), namespace, name).
