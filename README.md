# wireshark-falco
Create filtered pcap files from Falco Talon response actions
<br/><br/>
Create a dodgy, overprivleged workload:
```
kubectl apply -f https://raw.githubusercontent.com/nigel-falco/falco-talon-testing/main/dodgy-pod.yaml
```
```
kubectl exec -it dodgy-pod -- bash
```
Installing a suspicious networking tool like telnet
```
curl 52.21.188.179
```
