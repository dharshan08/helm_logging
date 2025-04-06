
# installation of helm chart

`kubectl create ns fluentd`

`kubectl create secret generic elasticsearch-credentials --from-literal=password='kibana'`

`kubectl create secret generic elasticsearch-credentials --from-literal=username='elastic' --from-literal=password='kibana' --namespace=fluentd`

`helm install my-logging-stack ./helm_logging -n fluentd`
 
# access kibana dashboard

http://<NODE-IP>:31601

