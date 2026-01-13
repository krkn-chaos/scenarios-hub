## scenarios-hub
Hosts scenario files for krkn which can be used for testing Kubernetes based frameworks and applications running on them.


### Supported configs
- [Kubernetes](kubernetes)
- [OpenShift](openshift)
- [CNV](cnv)


### Contributions
We are always looking for config additions from users on how they are leveraging Krkn to test Kubernetes based platforms and applications running on them. This will greatly help the community in reusing them to test their environements and expand them. Any contributions are most welcome.

### Using In Krkn
Clone both scenarios-hub and krkn under the same folder, then you can reference the scenario file sceanarios-hub in the krkn config like: 
```yaml
chaos_scenarios:
- pod_disruption_scenarios:
    - ../scenarios-hub/openshift/etcd.yml
```