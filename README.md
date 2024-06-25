# Service Mesh com Istio

### Instalação necessária

Dê preferência utilize o Linux ou Windows com WSL: 
https://k3d.io/v5.6.3/#installation

### Criando cluster

Rode o comando: `k3d cluster create -p "8000:30000@loadbalancer" --agents 2`.
> Será criado um cluster na porta 30000 com bind para sua máquina na porta 8000, juntamente com 2 agents/nodes.

E com o comando: `kubectl get nodes`, podemos ver o server que é a master e os 2 nodes.