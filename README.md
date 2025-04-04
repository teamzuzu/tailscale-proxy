# tailscale-proxy

a k8s deployment showing a simple approach to connecting your cluster to your headscale tailnet without having to use the operator

it includes haproxy so you can create services or whatever you want - a simple example exposing an opensearch cluster is included

pvc is used to store the tailscale state 

to deploy you need to update

- auth key ( in the auth-secret.yaml file  ) 
- headscale url ( TS_EXTRA_ARGS env var )
- cool name for your cluster ( TS_HOSTNAME env var in -depl) 
