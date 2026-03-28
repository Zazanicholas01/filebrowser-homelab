# k3s cluster manifests

This directory is populated from `/home/vagrant/manifests` during provisioning.

Suggested workflow inside the VM:
```bash
rsync -a --delete ~/manifests/ ~/Gitops_Homelab/clusters/k3s/
cd ~/Gitops_Homelab
git status
git add .
git commit -m "Sync manifests"
git push origin main
```
