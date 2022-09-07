# kube-infra-local
This repository represents my personal kubernetes clusters and their workloads. Flux handles keeping the cluster(s) up to date with the yamls in this repo via a pull configuration. To run your workload on my servers, submit a PR!

## Clusters
There's only 1 for now:

### local

| hostname | cpu | ram | storage | storage type | online? |
|:----------|:----------|:----------|:----------|:----------|:----------|
| mini01 | 4 cores | 16 GB | 256 GB | SSD | Yes |
| mini02 | 4 cores | 16 GB | 512 GB | SSD | No |

Kubeseal cert + oneliner:  
```kubeseal --cert https://raw.githubusercontent.com/Milkshak3s/kube-infra-local/main/clusters/local/sealed.cert <[input_secret] >[outout_sealedsecret]```

## Reserved Ports

| cluster | ports | reason |
|:--|:--|:--|
| local | 8001 | Persistent Outreach SS13 testing |
| local | 30008 | Persistent Outreach SS13 testing |
| local | 30009-40000 | General use |
