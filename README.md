
<p align="center">
    <img src="https://github.com/ondat/trousseau/blob/main/assets/logo-horizontal.png" >
</p>
<p align="center">
        <a href="https://lgtm.com/projects/g/ondat/trousseau/alerts/"><img alt="Total alerts" src="https://img.shields.io/lgtm/alerts/g/ondat/trousseau.svg?logo=lgtm&logoWidth=18"/></a>
      <a href="https://github.com/Trousseau-io/trousseau/actions/workflows/gosec-scanner-on-pull_request.yaml" alt="gosec">
        <img src="https://github.com/Trousseau-io/trousseau/actions/workflows/gosec-scanner-on-pull_request.yaml/badge.svg?branch=main" /></a>
      <a href="https://github.com/Trousseau-io/trousseau/actions/workflows/codeql-analysis.yml" alt="codeql">
        <img src="https://github.com/Trousseau-io/trousseau/actions/workflows/codeql-analysis.yml/badge.svg" /></a>
      <a href="https://github.com/Trousseau-io/trousseau/actions/workflows/go-lint-scan-pull_request.yaml" alt="golangci-lint">
        <img src="https://github.com/Trousseau-io/trousseau/actions/workflows/go-lint-scan-pull_request.yaml/badge.svg" /></a>
      <a href="https://bestpractices.coreinfrastructure.org/projects/5460" alt="CII Best Practices">
        <img src="https://bestpractices.coreinfrastructure.org/projects/5460/badge" /></a>
</p>

-----

**Please note**: We take security and users' trust seriously. If you believe you have found a security issue in Trousseau, *please responsibly disclose* by following the [security policy](https://github.com/ondat/trousseau/security/policy). 

-----

This is the home of [Trousseau](https://trousseau.io), an open-source project leveraging the [Kubernetes KMS provider framework](https://kubernetes.io/docs/tasks/administer-cluster/kms-provider/) to connect with Key Management Services the Kubernetes native way! 

* Website: https://trousseau.io 
* Announcement & Forum: [GitHub Discussions](https://github.com/ondat/trousseau/discussions)
* Documentation: [GitHub Wiki](https://github.com/ondat/trousseau/wiki)
* Hands-on lab: [Tutorial](https://www.ondat.io/trousseau)
* Recording of the hands-on lab: [DoK London Meetup](https://www.youtube.com/watch?v=BldQHinAIYg) 

## Why Trousseau

Kubernetes platform users are all facing the very same question: ***how to handle Secrets?***  

While there are significant efforts to improve Kubernetes component layers, [the state of Secret Management is not receiving much interests](https://fosdem.org/2021/schedule/event/kubernetes_secret_management/). Using *etcd* to store API object definition & states, Kubernetes secrets are encoded in base64 and shipped into the key value store database.  Even if the filesystems on which *etcd* runs are encrypted, the secrets are still not.   

Instead of leveraging the native Kubernetes way to manage secrets, commercial and open source solutions solve this design flaw by leveraging different approaches all using different toolsets or practices. This leads to training and maintaining niche skills and tools increasing cost and complexity of Kubernetes. 

Once deployed, Trousseau will enable seamless secret management using the native Kubernetes API and ```kubectl``` CLI usage while leveraging an existing Key Management Service (KMS) provider.   

How? By using using the [Kubernetes KMS provider](https://kubernetes.io/docs/tasks/administer-cluster/kms-provider/) framework to provide an envelop encryption scheme to encrypt secrets on the fly.

<p align="center">
    <img src="https://github.com/ondat/trousseau/blob/main/assets/Ondat%20Diagram-w-all.png" height="600">
</p>

## About the name
The name ***trousseau*** comes from the French language and is usually associated with keys like in ***trousseau de clés*** meaning ***keyring***.

## Contributing Guidelines
We love your input! We want to make contributing to this project as easy and transparent as possible. You can find the full guidelines [here](https://github.com/ondat/trousseau/blob/main/CONTRIBUTING.md).

## Community
Please reach out for any questions or issues via our [Github Discussions](https://github.com/ondat/trousseau/discussions).

Alternatively you can:
* Raise an issue or PR on this repo
* Follow us on Twitter [@ondat_io](https://twitter.com/ondat_io)

## Roadmap
You can view our project board [here](https://github.com/orgs/ondat/projects/1/views/4).

## License
Trousseau is under the Apache 2.0 license. See [LICENSE](https://github.com/ondat/trousseau/blob/main/LICENSE) file for details.
