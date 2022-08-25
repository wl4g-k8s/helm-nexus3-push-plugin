# Helm nexus3 repository plugin

A Helm plugin that pushes a chart directory or packaged chart tgz to a specified
Nexus Helm repo.

- Fork of [github.com/sonatype-nexus-community/helm-nexus-push](https://github.com/sonatype-nexus-community/helm-nexus-push)

## Installation

- `helm plugin install --version main https://github.com/wl4g-k8s/helm-nexus3-push-plugin.git`
- or: `helm plugin install --version main https://gitee.com/wl4g-k8s/helm-nexus3-push-plugin.git`
- `helm nexus-push --help`

## Usages

- `helm repo add --username myuser --password 123456 myrepo https://registry.your-domain.io/repository/helm-release/`
- `helm nexus-push myrepo mychart-0.0.1.tgz`
- `helm nexus-push myrepo ./mychart`

Additional help available `helm nexus-push --help`

## Updates

- `cd $HELM_HOME/plugins/nexus-push`
- `git pull`
- See to: `cat $HOME/.local/share/helm/plugins/helm-nexus3-push-plugin.git/push.sh`

## The Fine Print

It is worth noting that this is **NOT SUPPORTED** by Sonatype, and is a 
contribution of the community back to the open source community (read: you!)

Remember:

- Use this contribution at the risk tolerance that you have
- Do NOT file Sonatype support tickets related to Helm support in regard to this plugin
- DO file issues here on GitHub, so that the community can pitch in

Phew, that was easier than I thought. Last but not least of all:

Have fun creating and using this plugin and the Nexus platform, we are glad to have you here!

## Getting help

Looking to contribute to our code but need some help? There's a few ways to get information:

- Chat with us on [Gitter](https://gitter.im/sonatype-nexus-community/nexus-developers)
- Connect with us on [Twitter](https://twitter.com/sonatypeDev)
- Log an issue here on GitHub
