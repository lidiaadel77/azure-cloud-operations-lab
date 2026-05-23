
# Monitoring and Alerts

This file documents the monitoring configuration used in the Azure Cloud Operations Lab.

## Monitoring Goal

The goal of monitoring is to detect performance issues before they affect users.

## Azure Monitor

Azure Monitor was used to observe the virtual machine.

The main metric used in this lab was:

- Percentage CPU

## Alert Rule

Created an alert rule for high CPU usage.

Alert condition:

- Metric: Percentage CPU
- Condition: Greater than 80%
- Aggregation: Average
- Evaluation frequency: 5 minutes

## Why This Matters

High CPU usage can indicate:

- Heavy workload
- Application issue
- Background process problem
- Need for scaling or optimization

## Result

The alert rule helps detect high CPU usage on the VM and demonstrates basic cloud operations monitoring.
