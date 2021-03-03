# stackdriverShortURL

There is a needs to generate link to stackdriver logs:

https://console.cloud.google.com/logs/viewer?project=_PROJECT_&advancedFilter=resource.type%3D%22k8s_container%22%0Aresource.labels.cluster_name%3D%22_K8S_CLUSTER_NAME_%22%0Aresource.labels.namespace_name%3D%22_K8S_NAMESPACE_%22%0Aresource.labels.container_name%3D%22_K8S_CONTAINER_NAME_%22%0A(jsonPayload.request%3A%20%22PUT%20%2Finspectorio%2Fv2%2Fpos%2F%22)%0A(jsonPayload.request_time%3D~%22%5B1-9%5D%5B0-9%5D%5C.%22%20OR%20jsonPayload.request_time%3D~%22%5B2-9%5D%5C.%22)%0A&customFacets=jsonPayload.request_time%2CjsonPayload.request&limitCustomFacetWidth=false

do it with uniq_id. 

Sort url objects generated at deployment stage As ConfigMap
