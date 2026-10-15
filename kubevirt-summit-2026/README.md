# Secondary networks for KubeVirt VMs with DRA

KubeVirt Summit 2026, October 15, 2026 ·
[session page](https://sessionize.com/s/soren-henning/secondary-networks-for-kubevirt-vms-with-dra/190793)

**Slides:** [dra-sdn-kubevirt-summit.pptx](dra-sdn-kubevirt-summit.pptx)

Multus is the established way to give a pod or a KubeVirt VM a secondary network. Kubernetes Dynamic Resource Allocation (DRA), and KubeVirt's VEP-183 on top of it, open a second path. This talk compares both models side by side on Kube-OVN, with measurements: how each attaches a NIC, what the scheduler sees, how shared subnets and lifecycle work, and what hot-plug means for each.

## Code

- [kube-ovn-dra-driver](https://github.com/soer3n/kube-ovn-dra-driver): DRA driver for Kube-OVN (kubelet plugin and NRI hook)
- [kube-ovn-network-binding-plugin](https://github.com/soer3n/kube-ovn-network-binding-plugin): KubeVirt network binding plugin for the driver's NICs

## Status

- The slides are updated after the talk. The file keeps the same name, so links stay valid.
- A proposal to bring this into Kube-OVN is being prepared. Its link will be added here.
