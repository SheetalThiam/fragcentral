title: "- Fragmentation, centralization and consolidation "
abbrev: "- fragcentral"
category: info

docname: draft-todo-yourname-protocol-latest
submissiontype: IETF  # also: "independent", "editorial", "IAB", or "IRTF"

author:
 -
    fullname: Sheetal Kumar 
    Organization: Global Partners Digital 
    email: sheetal@gp-digital.org 

author:
 -
    fullname: Michaela Nakayama Shapiro 
    Organization: Article 19
    email: michaela.shapiro@article19.org

author:
 -
    fullname: Jessamine Pacis 

    Organization: Foundation for Media Alternatives 
    email: jpacis@fma.ph 
    


# Introduction

A defining feature of the internet is “its lack of any single point of technical, political, or economic control” [Nottingham 1]. However, that this model will continue to underpin the architecture of the Internet (as a “network of networks”) cannot be taken for granted, particularly as economic and political forces bear an increasing role on the Internet’s architecture and design. The values, as well as political and economic forces that are shaping the Internet’s architecture have been explored by the IETF through RFC 3935 [Alvestrand]. Reflections on the evolution of the end-to-end principle and the impact on the end-user are also the subject of multiple RFCs [Nottingham 2 ; Carpenter]
In particular, and facilitated by the decentralization of the internet group (DINRG), there has been a discussion of what constitutes consolidation and centralization at the IETF. There has also been a discussion of how consolidation and centralization relate to fragmentation (itself a contested term, as explored below). What is missing is an analysis of the impact these trends have on the end-user, as the reference point for the design of internet protocols at a time when economic and political forces are increasingly having an impact on how the internet evolves. 
To address this gap, this document assesses the current status of discussions relevant to centralization, consolidation and fragmentation at the IETF; recommends an approach for understanding the relevance and current status of these discussions focused on the end-user; and lays out a suggested set of use-cases (with recommendations for key points of analysis for an end-user centred approach).

# 2 Terminology 

2.1 Consolidation and centralization 

Consolidation has been discussed within DINRG interchangeably with centralization. However, it is important to distinguish between the two to understand whether and how internet protocol design intersects with broader economic and political forces. Here, we will attempt to set out the differences between the two concepts and make the case for the importance of clearly defining these terms to understand the potential impact on end-users. 

The terms "centralization" and "consolidation" have been used interchangeably at the IETF, even in texts relating to the definition of either centralization or consolidation. [McFadden; Huitema]. Both terms refer to the concentration of power - whether over consumers, the technical architecture underpinning the internet, financial, or otherwise [Lazanski]. However, within each term, there is a more granular understanding of how each can manifest, whether in operational impact, developmental, technical, etc. 

For example, discussions in previous I-Ds [Lazanski; McFadden], illustrate how consolidation is primarily concerned with market or economic trends and forces that impact the economy, and which can influence network and protocol design. This can encompass market concentration and security, DNS consolidation, and supply chains, with implications for interoperability and Internet architecture as well as end users. With regards to end-users, this means that mass collection of user data and their online behaviours are increasingly concentrated in the hands of a small number of big companies in a phenomenon known as “data consolidation.” At the same time, “centralization” has been defined as the state of affairs where a single entity or a small group of them can observe, capture, control, or extract rent from the operation or use of an Internet function [Nottingham 1]. The “result” of both centralization and consolidation trends share the following characteristics: fewer entities with more control, leading to a concentration of ‘choke points’, and the potential for single points of failure. The Internet Society provides a measurement of internet consolidation (referred to as "concentration" via its Pulse dashboard, utilising the Gini coefficient and the Herfindahl-Hirschman Index (HHI) to assess internet consolidation.

It is important to note that the concentration of economic forces has also been said to have a positive impact in so far as it has enabled investment in the internet’s evolution by increasing resources available and facilitating the development and implementation of key protocols: e.g the implementation of key protocols such as DNS-over-HTTPS which has provided privacy and security protection to end-users across the network [Lazanski] as well as investment into infrastructure and the services that ultimately impact consumers (including end-users). 

Therefore, any efforts to differentiate between the two terms largely come down to whether the impact on the network and the end-user arises primarily or solely from economic and market forces, the design or standards or protocols, or the capabilities permitted by standards and protocols. In distinguishing between the two, it is important to recognise that consolidation arises from external market and political forces and centralization could arise from creating or facilitating architectural changes at the protocol level, which may feed into and in turn shape external forces in some way. Therefore, whereas definitions of consolidation focus on  the outcome of the realities of the market, centralization is broader: and can be an outcome of protocol choices, or engineering decisions. 

We have examined what makes each term distinctive (consolidation’s focus on economic and political forces, centralization’s broader explanation for how standards arrive at the same outcome) and what each term shares (each lead to an entrenchment of choke points/points of control). To summarise, while the terms are used interchangeably, it is important to note distinguishing elements as well, because of the need to understand the relevance of the IETF’s mandate, e.g the development or evolution of internet standards and protocols in relation to the broader economic and political context, and current forces and trends.

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

These types of fragmentation do not operate in silos and are often interconnected.  For example, regulatory actions, such as efforts by governments to push users onto domestic networks, can lead to technical fragmentation: in the case of Iran, the government blocked domestic internet service provider’s (ISP) access to international gateways, which meant the global internet was centralised to only government-controlled getaways serving as the only access point for all international traffic and IP capacity and connectivity services in the country. These government-controlled getaways can facilitate censorship by preventing end-users in the country from accessing content hosted on international servers and forcing end-users to utilise servers that may expose identifiers [Article 19]. Such actions can also lead to technical fragmentation whereby the domestic internet infrastructure is no longer interoperable with that of the global internet. This has serious ramifications for freedom of expression online, negatively impacting end-users ability to access and share information [PNIF]. 

We also see this in efforts that aim to address consolidation but can inadvertently lead to fragmentation: for example, with EU proposals to enforce ‘sender-pay’ agreements, which impact the decentralised management of the internet (one of the critical properties) by altering the nexus of control over the technical architecture of the Internet by providing telecommunication providers with the ability to control traffic flows [GPD 2]. Increasing efforts to restrict data flows or control what data individuals can access online are also having an impact on the technical layer of the Internet. Network shutdowns, DNS-based blocking (among other censorship tools), firewalls, and walled gardens all represent efforts by governments to prevent users’ access to certain information, with potential impacts on the technical layer of the internet if more widely and consistently adopted. Such regulatory efforts to protect ‘digital sovereignty’ are leading to increasing politicisation of the internet’s core - meaning the fundamental technical functions that keep the internet functioning, such as the domain name and addressing system [GPD 1].

At IETF 117, two presentations are of particular interest to this draft, that of Nick Merrill and of Baltra. 

In the definition of internet fragmentation proposed by Baltra, the Internet is the connected component of more than 50% of the active, public IP addresses that can reach each other. In their paper they identify islands and peninsulas of connectivity, which could be seen as fragments and in their definition if none of the connected components reaches 50% of the active, public IP addresses then the network of networks is so fragmented that the Internet doesn't exist any longer. Using this definition means that the fragmentation of the Internet would be a binary event, whereby from one moment to another the Internet ceases to exist. As such, this is a narrow IP connectivity based perspective on fragmentation [Baltra].

Another way of measuring internet fragmentation has been proposed by Nick Merrill, whose research uses a set of proxy measures that correspond to specific layers of the internet stack, including: data laws (for the governance layer); website ranking locality (application layer); network interference events (transport layer), and IPV4 to IPV6 transition (network layer). His findings showed that the picture for the state of the Internet is complicated: the internet reflects and impacts geopolitical relationships, and is shaped by the ‘control points’ that impact how and what it routes. Control points refers to the various service providers and intermediaries that ensure that internet traffic flows to where it’s meant to go (or in cases of blocking / shutdowns, that content does not reach its destination). His presentation focuses on content distribution networks (CDNs) and how the market is concentrated in the hands of a few US-owned companies who hold extraordinary power over the content to which end-users have access and it is to this trend - the concentration of power held by US companies over the running of the internet - that those concerned with internet fragmentation are reacting [Merrill]. This measurement work has been conducted as part of the Daylight lab and is tracked on Github (https://github.com/daylight-lab/III). 

In addition, according to a draft I-D on internet fragmentation, Knodel suggests that the main concern relating to the internet fragmentation relates to internet norms and meaningful connectivity (similarly to the IGF PNIF’s framework), namely “when interconnected network departs so drastically from the norms of the rest of the Internet that from a user perspective it no longer functions as part of the internet, which can result in loss of meaningful connectivity to the internet [Knodel]. “Only measuring technical fragmentation, for example, is not enough if content flows are tightly controlled as in the case of China [Hawkins]. It is worth attempting an assessment framework to understand at what point a network is no longer considered to be effectively part of the internet. Or, perhaps, more practically, the ability to analyse a proposed legal or policy change that would "tip" a network from being open to being closed - need for technically grounded discussions”.

# 3 A framework for understanding the intersection from the perspective of the end-user 
3.1 An end user perspective: what does this mean?

Arguably, as stated in RFC 8890 [Nottingham 2], even before the IETF was established, the Internet technical community has focused on user needs [Crocker], which stated that "one of our goals must be to stimulate the immediate and easy use by a wide class of users." According to RFC 3935; central to the Mission of the IETF are the concepts of decentralised control, edge-user empowerment, and sharing of resources, which are “technical concepts” embraced by the IETF [Alvestrand]. RFC 8890 defines an “end user” of the Internet as a person who uses a web browser, mail client, or another agent that connects to the Internet. It also states that end users are human users whose activities IETF standards support, sometimes indirectly [Nottingham 2].

RFC 8890 stresses that the end user perspective is a complex one as end users are not a homogenous group. End users connect to the Internet for many different purposes and therefore “might have different views of how the Internet should work.” They also might have varying interests (e.g., privacy, security, flexibility, reachability) that may sometimes be in tension [Nottingham 2]. On the other hand, the concept of human rights has also been explored in relation to the end user: according to RFC8280, “An end user perspective is therefore one that takes as a major consideration the human rights impact of design decisions on their end users, based on established human rights protocol considerations” [Cath]. 

Elsewhere, according to the European Electronic Communications Code (EECC), “end-user” means a user not providing public electronic communications networks or publicly available electronic communications services. In turn, “user” means a natural or legal person using or requesting a publicly available electronic communications service. On that basis, BEREC understands “end-user” to encompass individuals and businesses, including consumers as well as content and application providers (CAPs).

3.2 End users and end-point architectures

The end-to-end principle and the way it impacts the end user is addressed in RFC1958, which states it is highly desirable that Internet carriers protect the privacy and authenticity of all traffic, but this is not a requirement of the architecture [Carpenter]. Confidentiality and authentication are the responsibility of end users and must be implemented in the protocols used by the end users. Endpoints should not depend on the confidentiality or integrity of the carriers. Carriers may choose to provide some level of protection, but this is secondary to the primary responsibility of the end users to protect themselves”.
However, as the end-to-end principle itself evolves, it is worth asking what the relationship of the end user to the principle, and to the development and evolution of relevant internet standards and protocols is - and how it could evolve. 

3.3 The end-to-end principle 

The end-to-end principle was originally articulated as where best to put functions in a system. According to RFC 3724: “to perform its services, the network maintains some state information….the volume of this state must be minimized” [Kempf]

The end-to-end principle holds that "the intelligence is end-to-end rather than hidden in the network" [Saltzer ; Carpenter].  The end-to-end principle is important for the robustness of the network and innovation.  Such robustness of the network is crucial to enabling human rights like freedom of expression. [Cath]

Preserving user choice is one of the more recent articulations of the end-to-end principle. For example, “primary focus of concern in the reduction in transparency due to the introduction of NATs and other address translation mechanisms in the Internet, and the consequences to the end-to-end principle of various scenarios involving full, partial, or no deployment of IPv6” [Kempf].

The end-to-end principle is being impacted as internet architecture changes [Zhang]. New, interposing elements that challenge it are about addressing trust issues arising from increase in users and the consequent “rise of third parties” or intermediaries- a critical change in the past few years. “The requirements of third parties often have little or nothing to do with technical concerns, but rather derive from particular commercial, social and legal considerations” [Kempf]. The same RFC states that “end user choice and empowerment, integrity of service, support for trust, and "good network citizen behaviour" are all properties that have developed as a consequence of the end-to-end principle.  Recognizing these properties in a particular proposal for modifications to the Internet has become more important than before as the pressures to incorporate services into the network have increased.  Any proposal to incorporate services in the network should be weighed against these properties before proceeding”.

3.4 Connecting the different frameworks and charting an end-user perspective framework 

The above analysis has set out different frameworks relating to centralization, consolidation and fragmentation, and provided a snapshot of RFCs that address how the end-to-end principle is evolving. According to IETF RFCs, not only is the end-to-end principle evolving, the position of the end user (whose needs, as consistently displayed in IETF RFCs, has been central to the work of the IETF) in relation to the end-to-end principle is also evolving. 

Centralization, consolidation and fragmentation are different and contested phenomena. Whether, how and to what extent they are happening, are - as is clear from the frameworks and analysis above - contested. Yet, what is common to each of these trends is a concern that the locus of control or power is being concentrated or otherwise put, that internet choke points (creating the opportunities for single points of failure) are being strengthened, and that this is having an impact not only on the internet’s architecture but also on the end user. 

# 4. Recommendations 

What we have done in this document is to address a gap in the literature in how the concepts of centralisation and internet fragmentation link together and what can reasonably be done within the scope/remit of the IETF/IRTF. Through analysis of key RFCs (9518, 8890 and 9620 in particular), we have worked to develop a set of guidance for considerations when developing internet protocols to ensure that the end-user perspective is integrated into protocol design processes. From this framework, we aim to promote developers and researchers working in the IRTF/IETF space to consider how their work could have a negative impact on end-users, with the focus here being on centralisation and the end-to-end principle. 

4.1 Framework for Assessing Protocols
Internet standards can either enable or curtail the exercise of end-user rights depending on how they are designed [OHCHR]. To promote the identification, prevention, mitigation and accounting for potentially adverse impacts on the end-user, we have outlined a framework below with key questions for developers to consider when assessing the potential impact of protocol design on the end-user. The aim for this framework is to promote end-user rights, control and choice and uphold the end-to-end principle through the development of protocols that aim to counter centralisation trends.  

These considerations are categorised as follows: (1) protecting the right to privacy and anonymity, (2) ensuring interoperability; (3) promoting internet integrity (4) securing the end-to-end principle 

_4.1.1 Protecting Privacy and Anonymity:_ Freedom of expression and the right to privacy/anonymity online are mutually reinforcing rights. Privacy is also a prerequisite to the meaningful exercise of freedom of expression for end-users, particularly online [Article 19]. It is therefore critical to integrate considerations on how protocol design may impact the right to privacy and anonymity in the development process. Questions for consideration include: 
	 - Right to Privacy: Did you have a look at the Guidelines in the Privacy Considerations for Internet Protocols [RFC6973] section 7? Does your protocol maintain the confidentiality of metadata? 			Could your protocol counter traffic analysis? Does your protocol adhere to data minimization principles? Does your document identify potentially sensitive data logged by your 				protocol and/or for how long that needs to be retained for technical reasons?
	 - Anonymity and pseudonymity: Does your protocol make use of identifiers? Are these identifiers persistent? Are they used across multiple contexts? Is it possible for the user to reset or 				rotate them without negatively impacting the operation of the protocol? Are they visible to others besides the protocol endpoints? Are they tied to real-world identities? Have 			you considered the Privacy Considerations for Internet Protocols [RFC6973], especially section 6.1.2?
	 - Confidentiality: Does the protocol expose the transmitted data over the wire? Does the protocol expose information related to identifiers or data? If so, what does it reveal to each protocol 			entity (i.e., recipients, intermediaries, and enablers) [RFC6973]? What options exist for protocol implementers to choose to limit the information shared with each entity? What 			operational controls are available to limit the information shared with each entity?
_4.1.3 Promoting Internet Integrity:_ Ensuring access to information as well as the protection of that information as it is transmitted across the network is integral to ensuring an internet that is developed in interest of the end-user. Internet protocols can either facilitate or block the free flow of information across the networks depending on their design; to ensure access to information, it is critical that information be transported securely, with the contents of data packets remaining intact and unchanged from end-to-end (e.g. with clear boundaries between the layers of the internet ‘stack’). To that end, areas to consider include: 
	 - Integrity: Does your protocol maintain, assure and/or verify the accuracy of payload data? Does your protocol maintain and assure the consistency of data? Does your protocol in any way allow 			for the data to be (intentionally or unintentionally) altered?
	 - Authenticity: Do you have sufficient measures to confirm the truth of an attribute of a single piece of data or entity? Can the attributes get garbled along the way (see security)? If 				relevant, have you implemented IPsec, DNS Security (DNSSEC), HTTPS and other Standard Security Best Practices?
	 - Security: Did you have a look at Guidelines for Writing RFC Text on Security Considerations [BCP72]? Have you found any attacks that are somewhat related to your protocol/specification, yet 			considered out of scope of your document? Would these attacks be pertinent to the human rights enabling features of the Internet (as described throughout this document)?

_4.1.2 Ensuring interoperability and innovation: _To counteract centralisation trends, internet protocols should be designed to promote interoperability and facilitate permissionless innovation. This allows for more competition in the market, and therefore more options for end-users to choose from. However, this should be coupled with the goal of facilitating user switching between implementations and deployments of the functions they define or enable. Targeting proprietary functions to improve interoperability and portability of specific features that are often used to lock users into a platform (ex: a format for lists of contacts in a social network) is another means of promoting end-user choice. [Nottingham 1]. Areas to assess include:
	 - Openness (heterogeneity): Does your protocol support heterogeneity by design? Does your protocol allow for multiple types of hardware? Does your protocol allow for multiple types of 				application protocols? Is your protocol liberal in what it receives and handles? Will it remain usable and open if the context changes?
	 - Openness (Open standards): Is your protocol fully documented in a way that it could be easily implemented, improved, built upon and/or further developed? Do you depend on proprietary code 				for the implementation, running or further development of your protocol? Does your protocol favor a particular proprietary specification over technically-equivalent competing 				specification(s), for instance by making any incorporated vendor specification “required” or “recommended” [RFC2026]? Do you normatively reference another standard that is not 			available without cost (and could you do without it)? Are you aware of any patents that would prevent your standard from being fully implemented [RFC8179] [RFC6701]?
	 - Adaptability: Is your protocol written in a modular fashion and does it facilitate or hamper extensibility? In this sense, does your protocol impact permissionless innovation? (See Open 				Standards)
_4.1.4 Securing the end-to-end principle: _The delegation of power on the network has a significant impact on the end-to-end-principle. Limiting dependencies on intermediaries (where feasible and desirable) and ensuring the distribution of functions on the internet and their governance can help maintain the end-to-end principle. Areas for consideration include:
	 - Intermediaries: Does your protocol depend on or allow for protocol specific functions at intermediary nodes?
	 - Content signals: Does your protocol include explicit or implicit plaintext elements, either in the payload or headers, that can be used for differential treatment? Is there a way minimise 				leaking of such data to network intermediaries? If not, is there a way for deployments of the protocol to make the differential treatment (including prioritisation of certain 				traffic), if any, auditable for negative impacts on net neutrality?
	 - Decentralization: Can your protocol be implemented without a single point of control? If applicable, can your protocol be deployed in a federated manner? Does your protocol create additional 			centralized points of control?
	 - Censorship Resistance: Does your protocol architecture facilitate censorship? Does it include "choke points" that are easy to use for censorship? Does it expose identifiers that can be used 			to selectively block certain kinds of traffic? Could it be designed to be more censorship-resistant? Does your protocol make it apparent or transparent when access to a resource 			is restricted and why it is restricted?

# 5. Use Cases 

5.1 IPV4 and 6 migration
	IPV6 intended to improve data integrity and privacy for end users 
	Full, partial or no deployment of IPV6
 
5.2 Internationalised domain names 

5.3 Intentional Network shutdowns 

5.4 Unintentional blackouts 

5.5 Sender pays agreements

5.6 Social media bans (X/Twitter, Tiktok)

5.7 Standards that could impact net neutrality 

5.8 Encrypted DNS protocols 

5.9 Introduction of NATs/other translation mechanisms (see RFC3724)

5.10 TLS Trust Expressions 

# 6. Informative References 

[Alvestrand] Alvestrand, H., “A Mission Statement for the IETF”, RFC 3935, October 2004, <https://datatracker.ietf.org/doc/html/rfc3935>

[Article 19 1] Article 19, “The Global Principles on Protection of Freedom of Expression and Privacy, Policy Brief, March 2017, <https://www.article19.org/resources/the-global-principles-on-protection-of-freedom-of-expression-and-privacy/>

[ Article 19 2] Article 19, “Iran: Tightening the Net 2020,” September 2020, <https://www.article19.org/wp-content/uploads/2020/09/TTN-report-2020.pdf>
 
[Badiei] Badiei, F., “Reviving Internet Decentralization Without Relying on the ‘B word’!” January 2024, <https://pulse.internetsociety.org/blog/reviving-internet-decentralization-without-relying-on-the-b-word> 

[Baltra] Baltra, G., “Improving network reliability using a formal definition of the Internet core,” IETF117,  July 2023, <https://play.conf.meetecho.com/Playout/?session=IETF117-HRPC-20230726-2000> 

[Carpenter] Carpenter, B., “Architectural Principles of the Internet,” RFC 1958, June 1996, <https://datatracker.ietf.org/doc/html/rfc1958>

[Cath] Cath, C., ten Oever, N., “Research into Human Rights Protocol Considerations,” RFC 8280, July 2020, <https://datatracker.ietf.org/doc/rfc8280/>

[Crocker] Crocker, S., “Host Software”, RFC 1, April 1969, <https://datatracker.ietf.org/doc/html/rfc1>

[Drake] Drake, W., Cerf, V., Kleinwächter, W., “Internet Fragmentation: An Overview,” World Economic Forum, January 2016, <https://www3.weforum.org/docs/WEF_FII_Internet_Fragmentation_An_Overview_2016.pdf>

[Global Partners Digital 1] Global Partners Digital, “Internet Fragmentation and Human Rights: How to counter threats to an open, interoperable and global Internet,” May 2024, <https://www.gp-digital.org/internet-fragmentation-and-human-rights-how-to-counter-threats-to-an-open-interoperable-and-global-internet/> 

[Global Partners Digital 2] Global Partners Digital, “Regional Roundtable Briefing: Internet Fragmentation and Human Rights in Europe,” February 2024,
<https://www.gp-digital.org/publication/regional-roundtable-briefing-internet-fragmentation-and-human-rights-in-europe/>

[Grover] Grover, G., Oever, N., “Guidelines for Human Rights Protocol and Architecture Considerations,” RFC 9620, September 2024, <https://datatracker.ietf.org/doc/rfc9620/>

[Hawkins] Hawkins, Z., “Internet Governance Doublespeak: Western Governments and the Open Internet,” Council on Foreign Relations, January 2023, <https://www.cfr.org/blog/internet-governance-doublespeak-western-governments-and-open-internet> 

[Huitema] Huitema, C., Huston, G., Kutscher, D., Zhang, L., “Report of 2021 DINRG Workshop on Centralization in the Internet, Computer Communication Review, July 2023, <https://dl.acm.org/doi/abs/10.1145/3610381.3610386#:~:text=The%20IRTF%20Research%20Group%20on,the%20above%20questions%20%5B1%5D >

[Internet Society] Internet Society, “The Internet Way of Networking: Defining the critical properties of the Internet”, Internet Way of Networking, 9 September 2020, < https://www.internetsociety.org/resources/doc/2020/internet-impact-assessment-toolkit/critical-properties-of-the-internet/>

[Internet Society] Internet Society, “Market Concentration”, <https://pulse.internetsociety.org/concentration>

[Kempf] Kempf, J., Austein, R., “The Rise of the Middle and the Future of End-to-End:
Reflections on the Evolution of the Internet Architecture”, RFC 3724, March 2004, < https://datatracker.ietf.org/doc/html/rfc3724>

[Knodel] Knodel, M., “On Internet Fragmentation,” draft I-D, October 2023, <draft-knodel-iab-fragmentation.md> 

[Lazanski] Lazanski, D., McFadden., “Protocol and Engineering Effects of Consolidation”, draft-lazanski-consolidation-05, April 2023, <https://datatracker.ietf.org/doc/draft-lazanski-consolidation/05/>

[McFadden] McFadden, M., “A Taxonomy of Internet Consolidation”, draft-mcfadden-consolidation-taxonomy-03, April 2024, <https://datatracker.ietf.org/doc/draft-mcfadden-consolidation-taxonomy/03/>

[Merrill] Merrill, N., “IETF 117 - Fragmentation & concentration: Beyond "free" & "closed," elsehow, August 2023, <https://www.else.how/p/ietf-117-fragmentation-and-concentration>

[Nottingham 1] Nottingham, M., “Centralization, Decentralization, and Internet Standards”, RFC 9518, December 2023, <https://datatracker.ietf.org/doc/rfc9518/>

[Nottingham 2] Nottingham, M, “The Internet is for End Users”, RFC8890, August 2020, <https://datatracker.ietf.org/doc/html/rfc8890> 

[OHCHR] Office of the United Nations High Commissioner for Human Rights, “Human rights and technical standard-setting processes for new and emerging digital technologies,” A/HRC/53/42, June 2023, <https://digitallibrary.un.org/record/4031373?ln=en&v=pdf>

[PNIF] Policy Network on Internet Fragmentation (PNIF), “PNIF Discussion Paper (input to IGF 2023),” Internet Governance Forum, September 2023, <https://www.intgovforum.org/en/filedepot_download/256/26218> 

[Zhang] Zhang, L., “Discussion: Is the End-to-End argument in system design still needed?,” DINRG, March 2023, <https://datatracker.ietf.org/meeting/116/materials/slides-116-dinrg-discussion-is-the-end-to-end-argument-in-system-design-still-needed-03> 

# Security Considerations

TODO Security


# IANA Considerations

This document has no IANA actions.


--- back

# Acknowledgments
{:numbered="false"}

TODO acknowledge.
