---

copyright:
  years: 2017, 2020
lastupdated: "2020-09-23"

keywords: IBM Blockchain Platform, release, new features, multicloud

subcollection: blockchain-sw-251

---

{:shortdesc: .shortdesc}
{:codeblock: .codeblock}
{:screen: .screen}
{:pre: .pre}
{:note: .note}
{:important: .important}
{:tip: .tip}
{:external: target="_blank" .external}

# What's new
{: #whats-new}

<div style="background-color: #f4f4f4; padding-left: 20px; border-bottom: 2px solid #0f62fe; padding-top: 12px; padding-bottom: 4px; margin-bottom: 16px;">
  <p style="line-height: 10px;">
    <strong>Running a different version of IBM Blockchain Platform?</strong> Switch to version
    <a href="/docs/blockchain-sw?topic=blockchain-sw-whats-new">2.1.2</a>,
    <a href="/docs/blockchain-sw-213?topic=blockchain-sw-213-whats-new">2.1.3</a>
    <a href="/docs/blockchain-sw-25?topic=blockchain-sw-25-whats-new">2.5</a>
    </p>
</div>


## August 27, 2020
{: #whats-new-08-19-2020}

The {{site.data.keyword.blockchainfull_notm}} Platform can now be deployed onto OpenShift clusters from the Red Hat Marketplace, an open cloud catalog that makes it easier to discover and access certified software. Red Hat certified {{site.data.keyword.blockchainfull_notm}} Platform operator images are available in the marketplace and accessible from your OpenShift web console. This new deployment option is immediately available to deploy on any Red Hat OpenShift 4.3+ cluster, and provides a fast, integrated experience for deploying the blockchain console that can be used to create Certificate Authorities (CAs), peers, and ordering nodes, in the public cloud. See [Deploying {{site.data.keyword.blockchainfull_notm}} 2.5 from Red Hat Marketplace](/docs/blockchain-sw-25?topic=blockchain-sw-25-deploy-ocp-rhm) for more information about this streamlined deployment option that is provided as an alternative to the existing [manual deployment](/docs/blockchain-sw-25?topic=blockchain-sw-25-deploy-ocp) steps.


## June 18, 2020
{: #whats-new-06-18-2020}


{{site.data.keyword.blockchainfull}} Platform 2.5 is now available.


{{site.data.keyword.blockchainfull_notm}} Platform 2.5 provides tighter integration with Red Hat solutions, including additional integration with Red Hat OpenShift 4.3 and support for Red Hat CodeReady Workspaces. This latest release also makes available a set of Ansible Content Collections to help accelerate the deployment of blockchain solutions.

**IBM Blockchain Platform Ansible Playbooks**  

The {{site.data.keyword.blockchainfull_notm}} Platform 2.5 improvements are designed to enable enterprises to launch production blockchain networks faster. This release helps organizations accelerate deployment through support of Ansible, an open source tool that automates provisioning, configuration management, and application deployment. **Ansible Content Collections** are packages of modules, plug-ins, and other Ansible content that automate these processes. The platform has published a set of Ansible Content Collections to help organizations deploy blockchain components and networks with greater speed. See [Getting started with Ansible playbooks on the {{site.data.keyword.blockchainfull_notm}} Platform](/docs/blockchain-sw-25?topic=blockchain-sw-25-ansible) to learn more.

**Red Hat CodeReady Workspaces**  

The platform expands its developer tool ecosystem with **Red Hat CodeReady Workspaces**, that help organizations speed up and simplify the setup of blockchain development environments. Red Hat CodeReady Workspaces provide a preconfigured and shared runtime environment that enables cloud-native blockchain development to be performed across teams. Red Hat CodeReady Workspaces offer strong security and adhere to enterprise-grade compliance for cloud-native development. Read about the [benefits of CodeReady Workspaces](/docs/blockchain-sw-251?topic=blockchain-sw-251-develop-vscode#develop-vscode-crw-why) to learn more.

**Hyperledger Fabric 2.0 images**

This release also includes improved usability and security by using **Hyperledger Fabric v2** and introduces the capability to deploy new peer and ordering nodes based on either Hyperledger Fabric v1.4.7 or v2.1.1. While all of the new Fabric v2 capabilities are not yet available on the platform, when you deploy a peer based on the Fabric v2.1.1 image, smart contracts are deployed into their own pod rather than inside a container on the peer pod, eliminating the dependency on the Docker daemon. Deploying peer and ordering nodes with the Fabric v2.x images is recommended to ensure that going forward you have access to the latest Fabric fixes and features. It is not currently possible to migrate existing nodes to Fabric 2.1.1 images.  The ordering service requires that all ordering nodes be running either Fabric v1.4.x or Fabric 2.x. Mixing ordering nodes with these different Fabric versions can introduce problems when attempting to update the consenter set. Peers, on the other hand can coexist on a channel even when they run different Fabric levels, as long as the channel application capability is not higher than the lowest peer Fabric version. 


If you have an existing {{site.data.keyword.blockchainfull_notm}} Platform v2.1.x deployment and are interested in upgrading to {{site.data.keyword.blockchainfull_notm}} Platform 2.5, see the following topics:
- [Upgrading your console and components on the OpenShift Container Platform](/docs/blockchain-sw-25?topic=blockchain-sw-25-upgrade-ocp)
- [Upgrading your console and components on Kubernetes](/docs/blockchain-sw-25?topic=blockchain-sw-25-upgrade-k8)
- [Upgrading the {{site.data.keyword.blockchainfull_notm}} images](/docs/blockchain-sw-25?topic=blockchain-sw-25-blockchain-images#blockchain-images-upgrade)



See the [Release notes](/docs/blockchain-sw-251?topic=blockchain-sw-251-release-notes-saas-20#06-18-2020) for more details on the new features that are included in this release.




