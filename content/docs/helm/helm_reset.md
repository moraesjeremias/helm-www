## helm reset

Uninstalls Tiller from a cluster

### Synopsis


This command uninstalls Tiller (the Helm server-side component) from your
Kubernetes Cluster and optionally deletes local configuration in
$HELM-HOME (default ~/.helm/)


```
helm reset [flags]
```

### Options

```
  -f, --force                 Forces Tiller uninstall even if there are releases installed, or if Tiller is not in ready state. Releases are not deleted.)
  -h, --help                  help for reset
      --remove-helm-home      If set, deletes $HELM-HOME
      --tls                   Enable TLS for request
      --tls-ca-cert string    Path to TLS CA certificate file (default "$HELM-HOME/ca.pem")
      --tls-cert string       Path to TLS certificate file (default "$HELM-HOME/cert.pem")
      --tls-hostname string   The server name used to verify the hostname on the returned certificates from the server
      --tls-key string        Path to TLS key file (default "$HELM-HOME/key.pem")
      --tls-verify            Enable TLS for request and verify remote
```

### Options inherited from parent commands

```
      --debug                           Enable verbose output
      --home string                     Location of your Helm config. Overrides $HELM-HOME (default "~/.helm")
      --host string                     Address of Tiller. Overrides $HELM-HOST
      --kube-context string             Name of the kubeconfig context to use
      --kubeconfig string               Absolute path of the kubeconfig file to be used
      --tiller-connection-timeout int   The duration (in seconds) Helm will wait to establish a connection to Tiller (default 300)
      --tiller-namespace string         Namespace of Tiller (default "kube-system")
```

### SEE ALSO

* [helm](../../docs/helm/#helm)	 - The Helm package manager for Kubernetes.

###### Auto generated by spf13/cobra on 16-May-2019