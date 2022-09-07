# kube-infra-local
This repository represents my personal kubernetes clusters and their workloads. Flux handles keeping the cluster(s) up to date with the yamls in this repo via a pull configuration. To run your workload on my servers, submit a PR!

## Clusters
There's only 1 for now:

### local
Machines

| hostname | cpu | ram | storage | storage type | online? |
|----------|----------|----------|----------|----------|----------|
| mini01 | 4 cores | 16 GB | 256 GB | SSD | Yes |
| mini02 | 4 cores | 16 GB | 512 GB | SSD | No |

## Reserved Ports

| cluster | ports | reason |
|--|--|--|
| local | 30008 | Persistent Outreach SS13 testing |
| local | 30010 | Sealed secret public cert |
| local | 30000-40000 | General use |
