# clone the repository
`https://github.com/dharshan08/helm_logging.git`

`cd helm_logging`

# packaging the helm chart
`helm package .`

# installation of helm chart

`kubectl create ns fluentd`

`helm install my-logging-stack ./my-logging-stack-0.1.0.tgz`

# set credentials
`kubectl create secret generic elasticsearch-credentials --from-literal=password='kibana'`

`kubectl create secret generic elasticsearch-credentials --from-literal=username='elastic' --from-literal=password='kibana' --namespace=fluentd`
