# tailscale-proxy

a k8s deployment showing a simple approach to connecting your cluster to your headscale tailnet without having to use the operator

to deploy you need to update

- auth key ( in the auth-secret.yaml file  ) 
- headscale url ( TS_EXTRA_ARGS env var )
- cool name for your cluster ( TS_HOSTNAME env var in -depl) 
