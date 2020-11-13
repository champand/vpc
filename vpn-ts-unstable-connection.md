---

copyright:
  years: 2018, 2020
lastupdated: "2020-11-13"

keywords: virtual private network, VPN, vpn gateway, troubleshooting

subcollection: vpc

---

{:tsSymptoms: .tsSymptoms}
{:tsCauses: .tsCauses}
{:tsResolve: .tsResolve}
{:shortdesc: .shortdesc}
{:screen: .screen}
{:support: data-reuse='support'}
{:codeblock: .codeblock}
{:pre: .pre}
{:note:.deprecated}
{:troubleshoot: data-hd-content-type='troubleshoot'}

# Why is my connection unstable?
{: #troubleshoot-unstable-connection}
{: troubleshoot}
{: support}

{: tsSymptoms}
My connection is not stable and keeps going down.

{: tsCauses}
There might be a rekey timing conflict.  

{: tsResolve}
Follow the steps to resolve any timing issues:

1. Make sure NAT-Traversal is enabled on the peer, if it is a configurable option.
1. If you are using IKEv2, try using different lifetimes so that the side with the shorter lifetime always initiates the rekeying process. 
1. Try disabling and re-enabling the connection.