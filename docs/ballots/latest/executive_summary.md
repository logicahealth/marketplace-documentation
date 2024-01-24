# A Call For Product Portability

#### Landscape
Products deployed in an enterprise are constituent building blocks in a larger information technology (IT) architecture. The deployment and runtime characteristics of each individual product and its underlying infrastructure naturally vary across organizations, requiring each deployed product to be further tailored to local IT needs. These processes of procurement and local configuration vary greatly across customers as an accepted part of "implementation time" and "total cost of ownership" (TCO) for incorporating a product into the enterprise. This lack of infrastructural pre-coordination can result in extremely long IT implementation cycles for any capability to be added to, or changed within, an architecture, especially when underlying infrastructure is completely proprietary to the local institution and/or vendor platform.

Burdens of local implementation are confounded by a rise in interest for portable, declarative clinical knowledge such as HL7 Fast Healthcare Interoperability Resources (FHIR) Clinical Reasoning, as well as libraries of directly executable clinical knowledge such as HL7 CDS Hooks services and HL7 Clinical Quality Language (CQL). Any reduction to time spent in the discovery, evaluation, procurement, implementation, and maintainence of a product within an enterprise service oriented architectures is of great value to the HIT community as a source of increasing architectural agility. For organizations willing to invest in automated deployment of such standards-based products, direct savings could be substantial. The Marketplace API specification serves as a building block for orchestrating the exchange of such portable products and computable knowledge.

#### The Next Generation

Newer standards, notably FHIR, FHIR implementation guidance (e.g. Substitutable Medical Applications Reusable Technologies or "SMART-on-FHIR"), CDS Hooks, CQL and similar standards present several double-edged swords to health IT (HIT).

The ability to decouple standard-based solutions from underlying data authorities allows for great flexibility and removes reliance on repetitious point-to-point negotiations of current product procurement proceesses, allowing application developers to focus on creating applications based on common, open APIs. SOAs can still experience explosive growth in integration complications due to the combinatorics of integrations, unfortunately; more so when connections span heterogeneous networks.

The intentional extensibilty of FHIR introduces risk of a standards-based health IT software market that is still not interoperable to a desired extent. The Marketplace API specification offers operators flexibility to innovate while also encouraging adoption of over-arching product principles in cybersecurity, pricing, customer transparency, software provenence, and other non-functional areas.

#### Product Software Development Life Cycles (SDLCs)

 <!-- There are many tradeoffs in the continuum between monolithic and microservice architectural principles, and the exponential increase in potential touch points in highly decoupled architectures is not to be discounted. Further, d -->

The release cycles of independent software vendors (ISV) that develop IT products rarely align with the maintenance and support practices of customer production environments, often resulting in update delays from years to decades if program managers batch changes from many vendor systems into periodic internal rollouts. Implementations of the Marketplace specification aim to lower these burdens by normalizing the idea of product "injection": automating updates to deployed services and content within live environments using principles of continuous deployment and delivery.

Pertaining to FHIR-oriented specifications such as SMART and CDS Hooks, consideration is paid to the ability of health systems to run hybrid SOA environments mixing on-premise data centers with cloud providers. Healthcare systems are already familiar with the benefits of cloud IaaS, but are rarely able to leverage it to boundless degree. A SMART UI application, for example, may need to be hosted locally due to VPN, DNS, or content filtering restrictions at the network level. Similarly, a CDS Hooks service may not be permitted to execute over the public Internet as a security policy, lack of suitable service level agreement (SLA), data use agreement (DUA), or infinite number of other concerns raised by CISOs and stakeholders.

Marketplace-level interoperability is not limited to "applications". Many types of standards-based products may be published and distributed by this specification, both within and external to the HL7 family of standards. In jurisdictions where regulatory boundaries have been drawn between "app store"-like systems and runtime platforms, this specification also serves to deliniate those boundaries between "marketplace" and runtime "platform".