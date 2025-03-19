
# installation of helm chart

`kubectl create ns fluentd`

`helm install my-logging-stack ./helm_logging -n fluentd`

# set credentials
`kubectl create secret generic elasticsearch-credentials --from-literal=password='kibana'`

`kubectl create secret generic elasticsearch-credentials --from-literal=username='elastic' --from-literal=password='kibana' --namespace=fluentd`
