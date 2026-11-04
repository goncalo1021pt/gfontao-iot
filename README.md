# gfontao-iot

GitOps source for Inception-of-Things Part 3.
Argo CD watches `manifests/` and deploys it to the `dev` namespace.

Switch the app version live:

```bash
sed -i 's/wil42\/playground:v1/wil42\/playground:v2/g' manifests/deployment.yaml
git commit -am "v2" && git push
```
