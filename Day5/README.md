# Day 5

## Lab - Deploying NodeJS Application from Openshift Webconsole
```

```

## Lab - Deploying ReactJS Application from CLI
```
```

## Info - Installing NFS Server in Ubuntu
```
sudo apt install -y nfs-kernel-server
sudo systemctl start nfs-kernel-server.service
sudo apt install -y nfs-common
sudo systemctl restart nfs-kernel-server
sudo systemctl enable nfs-kernel-server
```

## Info - Openshift Network Policy
<pre>
- is essentially Kubernetes NetworkPolicy with some OpenShift-specific integrations
- is the primary mechanism for controlling network traffic between pods (and to/from external endpoints) 
  at L3/L4 level (IP addresses, ports, protocols)
- by default, pods in a namespace can talk freely to each other and to the outside world unless some Network Policy prevents it
- When we create a Network Policy for a particular Project(Namespace), all Pods in that Project(Namespace) 
  are isolated from the ingress(incoming) traffic 
- Only traffic that are allowed by explicit Network policiy are permitted 
- Multiple Policies in the same namespace(project) are combined(ORed together) 
</pre>
