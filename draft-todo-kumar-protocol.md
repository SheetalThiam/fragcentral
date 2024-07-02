---
###
# Internet-Draft Markdown Template
#
# Rename this file from draft-todo-yourname-protocol.md to get started.
# Draft name format is "draft-<yourname>-<workgroup>-<name>.md".
#
# For initial setup, you only need to edit the first block of fields.
# Only "title" needs to be changed; delete "abbrev" if your title is short.
# Any other content can be edited, but be careful not to introduce errors.
# Some fields will be set automatically during setup if they are unchanged.
#
# Don't include "-00" or "-latest" in the filename.
# Labels in the form draft-<yourname>-<workgroup>-<name>-latest are used by
# the tools to refer to the current version; see "docname" for example.
#
# This template uses kramdown-rfc: https://github.com/cabo/kramdown-rfc
# You can replace the entire file if you prefer a different format.
# Change the file extension to match the format (.xml for XML, etc...)
#
###
title: "TODO - Fragmentation, centralization and consolidation "
abbrev: "TODO - fragcentral"
category: info

docname: draft-todo-yourname-protocol-latest
submissiontype: IETF  # also: "independent", "editorial", "IAB", or "IRTF"
number:
date:
consensus: true
v: 3
area: AREA
workgroup: WG Working Group
keyword:
 - next generation
 - unicorn
 - sparkling distributed ledger
venue:
  group: WG
  type: Working Group
  mail: WG@example.com
  arch: https://example.com/WG
  github: USER/REPO
  latest: https://example.com/LATEST

author:
 -
    fullname: Sheetal Kumar 
    organization: Your Organization Here
    email: sheetal@gp-digital.org 

normative:

informative:


--- abstract

TODO Abstract


--- middle

# Introduction

TODO A defining feature of the internet is “its lack of any single point of technical, political, or economic control” [Nottingham 1]. However, that this model will continue to be what underpins the architecture of the Internet (as a “network of networks”) cannot be taken for granted, particularly as economic and political forces bear an increasing role on the Internet’s architecture and design. The values, as well as political and economic forces that are shaping the Internet’s architecture have been explored by the IETF through RFC 3935 [Alvestrand]. Reflections on the evolution of the end-to-end principle and the impact on the end-user are also the subject of multiple RFCs [Nottingham 2 ; Carpenter]
In particular, and facilitated by the decentralization of the internet group (DINRG), there has been a discussion of what consolidation and centralization is at the IETF. There has also been a discussion of how consolidation and centralization relate to fragmentation (itself a contested term, as explored below). What is missing is an analysis of the impact these trends have on the end-user, as the reference point for the design of internet protocols at a time when economic and political forces are increasingly having an impact on how the internet evolves. 
To address this gap, this document assesses the current status of discussions relevant to centralization, consolidation and fragmentation at the IETF; recommends an approach for understanding the relevance and current status of these discussions that is  focused on the end-user, and lays out a suggested set of use-cases (with recommendations for key points of analysis for an end-user centred approach).

# 2.1 Terminology 
Consolidation has been discussed within DINRG interchangeably with centralization. However, in order to understand whether and how internet protocol design intersects with broader economic and political forces, it is important to distinguish between the two. Here we will attempt to set out the differences between the two concepts and make the case for the importance of clearly defining these terms in order to understand the potential impact on end-users. 
IETF literature so far displays a lack of taxonomic consistency in the use of the terms centralization and consolidation. They are used interchangeably, even in texts relating to the definition of either centralization or consolidation. [McFadden; Huitema]. Both terms refer to concentration of power - whether over consumers, the technical architecture underpinning the internet, financial, or otherwise [Lazanski]. However, within each term, there is a more granular understanding of how each can manifest, whether in operational impact, developmental, technical, etc. 
For example, discussions in previous I-Ds [Lazanski; McFadden], illustrate how consolidation is primarily concerned with market or economic trends and forces that impact the economy, and which can influence network and protocol design. This can encompass market concentration and security, DNS consolidation, and supply chains, with implications for interoperability and Internet architecture as well as end users. With regards to end-users, this means that mass collection of user data and their online behaviours are increasingly concentrated in the hands of a small number of big companies in a phenomenon known as “data consolidation.” At the same time, “centralization” has been defined as the state of affairs where a single entity or a small group of them can observe, capture, control, or extract rent from the operation or use of an Internet function [Nottingham 1]. The “result” of both centralization and consolidation trends share the following: fewer entities with more control, leading to a concentration of ‘choke points’, and the potential for single points of failure. 
It is important to note that the concentration of economic forces has also been said to have a positive impact in so far as it has enabled investment in the internet’s evolution by increasing resources available and facilitating the development and implementation of key protocols: e.g the implementation of key protocols such as DNS-over-HTTPS which has provided privacy and security protection to end-users across the network [Lazanski] as well as investment into infrastructure and the services that ultimately impact consumers (including end-users). 
Therefore, any efforts to differentiate between the two terms largely comes down to whether the impact on the network and the end-user arises primarily or solely from economic and market forces, or also from the design or standards or protocols or the capabilities permitted by standards and protocols. Therefore, in distinguishing between the two, it is important to recognise that consolidation arises from external market and political forces and centralization could arise from creating or facilitating architectural changes at the protocol level, which may feed into and in turn shape external forces in some way. Therefore, whereas definitions of consolidation focus on  the outcome of the realities of the market, centralization is broader: and can be an outcome of protocol choices, or engineering decisions. 
We have examined what is singular/distinctive when it comes to the terms (consolidation’s focus on economic and political forces, centralization’s broader incorporating of how standards can be brought to bear on the same) and what is shared (each lead to an entrenchment of choke points/points of control). To summarise, while the terms are used interchangeably, it is important to note distinguishing elements as well, because of the need to understand the relevance of the IETF’s mandate, e.g the development or evolution of internet standards and protocols in relation to the broader economic and political context, and current forces and trends.
2.2 Internet fragmentation 
There is no one definition of internet fragmentation. In this section, current frameworks and definitions are summarised, in order to form the basis of the following analysis, which examines commonalities between discussions on internet fragmentation, centralization and consolidation and posits a common ‘theme’ or area of concern for continued examination. 
The World Economic Forum framework was developed in 2016 and is composed of three parts or ‘types of fragmentation’, which - it is said - are either happening to various degrees or could happen (should certain conditions be met). These are: technical fragmentation; governmental fragmentation and commercial fragmentation [Drake]. 
Technical fragmentation refers to conditions in the underlying infrastructure that impede the ability of systems to fully interoperate and exchange data packets and of the Internet to function consistently at all endpoints. According to the framework, this can happen within four areas: internet addressing; interconnection; naming and security. 
Governmental fragmentation refers to government policies and actions that constrain or prevent certain uses of the Internet to create, distribute, or access information resources. Examples include content and censorship; e-commerce and trade; national security; privacy and data protection; data localization; and fragmentation as an overarching national strategy (e.g cyber sovereignty).
Commercial fragmentation refers to business practices that constrain or prevent certain uses of the Internet to create, distribute, or access information resources. Examples include peering and standardization; network neutrality; walled gardens; geo-localization and geo-blocking; and infrastructure-related intellectual property protection. The above types of fragmentation vary and can either 1) exist or be a threat 2) be intentional or unintentional in its impact (which can be deep or shallow).
The WEC framework does not position the end user in  its framework. In its reference to technical interoperability it refers to ‘universal connectivity among the willing’ as the basis for interoperability or the ability to transfer and make usable data between systems and applications, and it is achieved via the deployment of common technical standards and protocols. However, ‘coherency and consistency from an end user standpoint’ are identified as important for avoiding fragmentation.
The IGF’s Policy Network on Internet Fragmentation framework (2023) provides a basis for conceptualising fragmentation and sees fragmentation as having three ‘dimensions’: user experience; technical and governance [PNIF]. 
User experience is  the phenomenon by which different end-users of the Internet, when trying to perform the same action online, are presented with different content, options or interfaces. It is when such fragmentation is forced upon the end-user by other parties, or when it hampers the communication among end-users and their ability to access content and services, that it can deny the advantages and the freedoms that the Internet is supposed to offer.
Technical fragmentation refers to a  range of challenges to interoperability at the transport layer that makes the Internet work as a medium of communications globally. The following practices may impact the Internet’s interoperability and as such lead to a fragmentation of the technical infrastructure: actions that have a negative impact on the critical properties of the internet [Internet Society]; the concentration or consolidation of internet resources for routing traffic; and interventions in the technical transport layer to mitigate issues in the content layer. The framework recognises that the extent to which technical fragmentation is happening or there is a risk of it happening is contested. 
Finally, governance fragmentation in the PNIF framework relates to the interactions between global Internet governance and standards bodies. It results in siloed or duplicative discussions and exclusion of specific groups from participation, duplicative or clashing standards/norms and thus creates possible impacts on the technical layer and on the end user. 
The PNIF framework includes “the user experience” as a central component. Importantly, the definition of user experience includes an element of ‘control’, or not being allowed choice with regards to the access of content that is allowed elsewhere; in other words access to information that mirrors territorial boundaries. The end user can and is impacted by technical fragmentation as described in the framework (due to the impact on global interoperability of the internet for example), but the means by which they are or could be impacted is not fully explored in the framework. In the governance component of the framework, the choice and capacities of end users is understood as limited by practices that undermine access to governance and decision making spaces [PNIF]. 

# Conventions and Definitions

{::boilerplate bcp14-tagged}


# Security Considerations

TODO Security


# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.
