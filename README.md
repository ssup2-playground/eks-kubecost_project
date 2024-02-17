# eks-kubecost Project

eks-cicd-dr is prototyping project for testing various architecture with kubecost and EKS.

## Prometheus Architecture

<img src="/images/architecture_prom.png" width="600"/>

Prometheus Architecture is the most commonly used basic architecture when using kubecost. Metrics required for cost calculation in Kubecost and cost metrics provided by Kubecost are collected by Prometheus. Additionally, when kubecost retrieves Cost Metric for cost visualization, it also retrieves it from Prometheus.

## Prometheus AMPCost Architecture

<img src="/images/architecture_prom_ampcost.png" width="800"/>

## Prometheus AMP

<img src="/images/architecture_prom_amp.png" width="800"/>

## ADOT Collector AMP Architecture

<img src="/images/architecture_adot_amp.png" width="800"/>

## AMP Architecture

<img src="/images/architecture_amp.png" width="800"/>
