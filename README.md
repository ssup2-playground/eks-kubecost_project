# eks-kubecost Project

eks-cicd-dr is prototyping project for testing various architecture with kubecost and EKS.

## Prometheus Architecture

<img src="/images/architecture_prom.png" width="600"/>

"Prometheus Architecture" is the most commonly used basic architecture when using kubecost. 

* Metrics required for cost calculation in Kubecost and cost metrics provided by Kubecost are collected by Prometheus.
* Kubecost retrieves cost metrics from Prometheus when visualizing cost.

## Prometheus AWS AMP Cost Architecture

<img src="/images/architecture_prom_ampcost.png" width="800"/>

"Prometheus AWS AMP Cost Architecture" is an architecture that centralizes only cost metrics in AWS AMP. It can be used when you want to visualize the cost of multiple EKS clusters while optimizing the cost of using AWS AMP.

## Prometheus AWS AMP

<img src="/images/architecture_prom_amp.png" width="800"/>

"Prometheus AWS AMP Architecture" is the basic architecture for linking Kubecost and AWS AMP.

* Metrics required for cost calculation in Kubecost and cost metrics provided by Kubecost are collected by Prometheus.
* Prometheus writes collected metrics to AWS AMP.
* Kubecost retrieves cost metrics from AWS AMP when visualizing cost.

## ADOT Collector AWS AMP Architecture

<img src="/images/architecture_adot_amp.png" width="800"/>

## AWS AMP Architecture

<img src="/images/architecture_amp.png" width="800"/>
