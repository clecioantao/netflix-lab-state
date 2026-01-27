# netflix-lab-state

State repo (GitOps) para o laboratório Netflix-like em kind.

Estrutura:
- `clusters/netflix-lab/root-app.yaml`: Root Application (App-of-Apps)
- `clusters/netflix-lab/apps/`: kustomizations por domínio (edge / apps)

Como usar:
1) Suba este repo para o Git (GitHub/Gitea).
2) Edite `repoURL` em `clusters/netflix-lab/root-app.yaml`.
3) Aplique o root app no cluster:
   `kubectl apply -f clusters/netflix-lab/root-app.yaml`
