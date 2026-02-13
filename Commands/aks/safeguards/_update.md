# [Command] _aks safeguards update_

Update a deploymentSafeguard

## Versions

### [2025-07-01](/Resources/mgmt-plane/L3tyZXNvdXJjZXVyaX0vcHJvdmlkZXJzL21pY3Jvc29mdC5jb250YWluZXJzZXJ2aWNlL2RlcGxveW1lbnRzYWZlZ3VhcmRzL2RlZmF1bHQ=/2025-07-01.xml) **Stable**

<!-- mgmt-plane /{resourceuri}/providers/microsoft.containerservice/deploymentsafeguards/default 2025-07-01 -->

#### examples

- Update a DeploymentSafeguards resource to Enforce level by managed cluster id
    ```bash
        aks safeguards update --managed-cluster subscriptions/subid1/resourceGroups/rg1/providers/Microsoft.ContainerService/managedClusters/cluster1 --level Enforce
    ```

- Update a DeploymentSafeguards resource with resourceGroup and clusterName arguments
    ```bash
        aks safeguards update -g rg1 -n cluster1 --level Enforce
    ```

- Update a DeploymentSafeguards resource to add excluded namespaces
    ```bash
        aks safeguards update -g rg1 -n cluster1 --excluded-ns ns1 ns2
    ```
