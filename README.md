This sets up a fluentd daemonset that runs on every node in the cluster and 
forwards all the container logs to a graylog cluster

On Openshift you will need to run the following:
```
oc adm policy add-scc-to-user privileged system:serviceaccount:kube-system:fluentd-graylog
```

