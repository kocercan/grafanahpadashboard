# Kubernetes HPA & Pod Count Dashboard

This repository contains a Grafana dashboard for monitoring Kubernetes Horizontal Pod Autoscaler (HPA) and pod counts. The dashboard provides insights into the desired and current replicas, CPU utilization, and pod statuses.

## Dashboard Overview

The dashboard includes the following panels:

- **Desired Replicas**: Shows the desired number of replicas for the selected HPA.
- **Current Replicas**: Displays the current number of replicas for the selected HPA.
- **Min Replicas**: Shows the minimum number of replicas configured for the selected HPA.
- **Max Replicas**: Displays the maximum number of replicas configured for the selected HPA.
- **CPU Utilization (%)**: Provides a graph of CPU utilization for the selected workload.
- **Running Pods**: Shows the number of running pods in the selected namespace.

## Screenshot

![2024-12-05_13-12_1](https://github.com/user-attachments/assets/f20eb5bc-4803-44ef-8c08-010b436019ea)


## How to Use

1. **Import the Dashboard**:
   - Download the JSON file from this repository.
   - In Grafana, go to `Dashboards` -> `Manage` -> `Import`.
   - Upload the JSON file and configure the data source.

2. **Configure Variables**:
   - After importing, configure the variables (`datasource`, `namespace`, `workload`) using the dropdown menus at the top of the dashboard.

3. **Explore Metrics**:
   - Use the dropdown menus to select the desired data source, namespace, and workload.
   - Explore the metrics and insights provided by the dashboard.

## Requirements

- Grafana 8.0+
- Prometheus with Kubernetes metrics
- Kubernetes Metrics Server

## Contributing

Contributions are welcome! Please feel free to submit a pull request or open an issue if you have any suggestions or improvements.

## License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for details.
