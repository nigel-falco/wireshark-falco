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

## Test commands for demo purposes
Find AWS Credentials
```
grep "aws_secret_access_key" /path/to/some/file
```
Read sensitive file untrusted
```
sudo cat /etc/shadow > /dev/null
```
Kubernetes Client Tool Launched in Container
```
apt-get update
apt-get install -y curl
curl -LO "https://dl.k8s.io/release/$(curl -L -s https://dl.k8s.io/release/stable.txt)/bin/linux/amd64/kubectl"
chmod +x kubectl
mv kubectl /usr/local/bin/
kubectl version --client
```
Detect reconnaissance scripts
```
bash -c ./LinEnum.sh
```
