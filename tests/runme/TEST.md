# Test Linkerd Docs

This markdown document helps to test the Linkerd docs.

First make sure the right Kubernetes version is installed:

```sh { name=kubectl-version }
kubectl version --short
```

then validate Linkerd install:

```sh { name=linkerd-version }
linkerd version
```

lastly, kick of the tests via:

```sh { name=test }
npx bats $GITHUB_WORKSPACE/tests/runme/getting-started.bats
```