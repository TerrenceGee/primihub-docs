---
sidebar_position: 2
---

# Scalability

*** What can PrimiHub extend? ***

![Extensilbe](./extensilbe-layer.svg)

PrimiHub can be extended in the following ways.

## Data Source Access Extension

PrimiHub supports different types of data sources to register as data sets in the PrimiHub resource network. Users can use the data source extension framework to encapsulate their own data sources and access the PrimiHub private computing network.

## Data Consumption Extension
The resulting data generated by privacy computing can be used for user-defined downstream data consumption through data consumption extensions.

## Access Application Extension

Through a common application interface, PrimiHub can support external application access for big data, machine learning, IoT and other scenarios.

## Syntax Layer Extension
Support to extend different languages to write complex privacy computing tasks.

:::tip

Currently PrimiHub only supports Protobuf and Python

:::

## Semantic Layer Extension

* According to the semantics (context) of multi-party security, the semantic layer parser infers which task scheduling to use and creates different types of schedulers
* The scheduler starts Woker on distributed nodes according to the assigned task type
* Distributed node workers start corresponding tasks according to their assigned semantics
* Task run using the selected protocol

## Protocol Layer Extension

The term "security protocol" is used here. Protocol extensions correspond to upper layer Task extensions, including ABY3, PSI, PIR, cheeth, secure xgboost, etc. Cryptographic engineers can develop custom security protocols according to protocol specifications and access PrimiHub platform

 
:::tip 

See[Security Protocol Development Guide] for how to extend security protocols.(developer-docs/protocol-dev-guide.md)

:::