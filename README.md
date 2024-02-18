# eks-kubecost Project

eks-cicd-dr is prototyping project for testing various architecture with kubecost and AWS EKS.

## Prometheus Architecture

<img src="/images/architecture-prom.png" width="600"/>

"Prometheus Architecture" is the most commonly used basic architecture when using kubecost. 

* Metrics required for cost calculation in Kubecost and cost metrics provided by Kubecost are collected by Prometheus.
* Kubecost retrieves cost metrics from Prometheus when visualizing cost.

## Prometheus AWS AMP Cost Architecture

<img src="/images/architecture-prom-ampcost.png" width="800"/>

"Prometheus AWS AMP Cost Architecture" is an architecture that centralizes only cost metrics in AWS AMP. It can be used when you want to visualize the cost of multiple AWS EKS clusters while optimizing the cost of using AWS AMP.

* Metrics required for cost calculation in Kubecost and cost metrics provided by Kubecost are collected by Prometheus.
* Kubecost retrieves cost metrics from Prometheus when visualizing cost.
* Prometheus writes cost metrics to AWS AMP

## Prometheus AWS AMP Architecture

<img src="/images/architecture-prom-amp.png" width="800"/>

"Prometheus AWS AMP Architecture" is the basic architecture for linking Kubecost and AWS AMP.

* Metrics required for cost calculation in Kubecost and cost metrics provided by Kubecost are collected by Prometheus.
* Prometheus writes collected metrics to AWS AMP.
* Kubecost retrieves cost metrics from AWS AMP when visualizing cost.

## ADOT Collector AWS AMP Architecture

<img src="/images/architecture-adot-amp.png" width="800"/>

"ADOT Collector AWS AMP Architecture" is an architecture in which ADOT collector replaces the metric collection role previously performed by Prometheus.

* Metrics required for cost calculation in Kubecost and cost metrics provided by Kubecost are collected by ADOT collector.
* ADOT collector writes collected metrics to AWS AMP.
* Kubecost retrieves cost metrics from AWS AMP when visualizing cost.

## AWS AMP Architecture

<img src="/images/architecture-amp.png" width="800"/>

"AWS AMP Architecture" is an agentless architecture that does not install agents to collect AWS EKS Cluster metrics using AWS AMP's Scrapper

* Metrics required for cost calculation in Kubecost and cost metrics provided by Kubecost are collected by AWS AMP Scrapper.
* Kubecost retrieves cost metrics from AWS AMP when visualizing cost.
