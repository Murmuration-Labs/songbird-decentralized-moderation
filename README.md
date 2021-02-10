# Songbird: Decentralized Content Moderation &amp; Assessment Proposal

## What Is This Document?

This document is presented as an idea sketch for how a decentralized content moderation and assessment system *might work*, as applied to social networks potentially built on top of distributed storage systems like IPFS. The information contained in this document is intended as a preliminary study only, and not a finished specification or proposal. It's goal is to spark conversations within the greater dweb community about these important issues, and to inspire improvements to and innovations upon the ideas discussed here. Feedback is strongly encouraged!

## Summary

* Songbird is a proposed model for a pluralistic, decentralized content moderation and assessments system, which can be applied to social networks (or other types of content-based networks) equally by all actors within a technological ecosystem.
* Songbird supposes that having many diverse actors incentivized to make and pool quality content assessment and moderation choices, instead of a single platform authority, will provide a more rich and customizable experience for users.
* Under the proposed Songbird model of decentralized moderation, all ecosystem actors have parity; they have the same rights and abilities to fine-tune content settings in line with their values. They can make, share, receive, and subscribe to content assessments and moderation or filtering actions.
* Songbird as a framework is adaptable in that aspects of it could be implemented to varying degrees in either decentralized, centralized, or hybrid systems. 
* The description contained here pre-supposes IPFS as a foundational layer, because the ability to link content assessments and moderation actions to unique persistent content-addressed names (i.e., ContentIDs or CIDs) would be of great value in such a system.

## Human Rights Context

* Songbird is modeled as an attempt to create a pluralistic rights-based technology which distributes decision-making power about content assessments and moderation or filtering actions laterally to all actors in an ecosystem, as opposed to a singular top-down centralized model. It allows users to technologically express their values.
* In particular, Songbird takes inspiration from a few key elements of international declarations such as the [UN Declaration of Human Rights](https://www.un.org/en/universal-declaration-human-rights/), and the [Charter of Fundamental Rights of the European Union](https://www.europarl.europa.eu/charter/pdf/text_en.pdf), as well as other similar documents. Selected excerpts are highlighted below, included for their potential relevance to the development of rights-based technologies. *Many other variations exist in international law, and these are presented for illustrative purposes only.*
  * *“All human beings are born free and equal in dignity and rights.”* (Art. 1, UNDHR)
  * *“Everyone has the right to respect for his or her physical and mental integrity.”* (Art. 3, CFREU)
  * *“No one shall be subjected to torture or to cruel, inhuman or degrading treatment or punishment.”* (Art. 5, UNDHR)
  * *“Everyone has the right to respect for his or her private and family life, home and communications.”* (Art. 7, CFREU)
  * *“Everyone has the right to freedom of thought, conscience and religion (...) either alone or in community with others and in public or private, [and] to manifest (...) in teaching, practice, worship and observance.”* (Art. 18, UNDHR)
  * *“Everyone has the right to freedom of expression … (and) freedom to hold opinions and to receive and impart information and ideas without interference by public authority (...)”* (Art. 11, CFREU)


## How Songbird Might Work

* In a technological ecosystem based on Songbird, all actors would have parity: the same abilities to express their fundamental rights by assessing content and taking resulting content moderation and filtering actions if they desire. Those abilities would include, at minimum:
  * Active local filtering, where an actor assesses content and chooses to filter out that content for themselves (or for their platform) for a given reason.
  * Collaborative filtering, where actors can share local filtering choices with one another peer-to-peer, or with subscribers, or by submitting reports to platforms or third parties for review.
  * Passive filtering, where actors can receive and automatically act on filtering signals received from peers or from actors to whom they subscribe.
* In practice, example use cases might look like:
  * Active local filtering: a user discovers and reactively adds undesirable CIDs to a local filter list for restriction (i.e., Actors make content assessments about CIDs)
  * Collaborative filtering: users share personal filtering results with one another (which are then acted on passively/automatically) (i.e., Actors share content assessments about CIDs with peers.)
  * Passive filtering: a user subscribes to an “official” source of their choosing which filters out certain content or types of content automatically on their behalf (Actors receive content assessments about CIDs from peers.)
  
## At the App & Platform Level
  
* For apps and platforms, it should be remembered that they too have rights of freedom of expression and the need to protect the integrity of their service in order to be able to continue delivering it. So, active local filtering might be applied by administrators to the part of the network accessible to or controlled by the service, according to their Terms, content policies, and applicable law.
  * Apps/platforms, in effect, would become one of many “assessors” of content and potential sources of content moderation and filtering actions, to which users of the service can subscribe (or in certain ToS or legal compliance cases may be required to subscribe). 
    * Ideally, at minimum, “official” assessments and moderation actions taken against a specific CID by an app or platform would be transparently made public by the app or platform to its users. 
    * One means to make them publicly available would be locally within the app. It would likely be desirable that they additionally be broadcast to other actors in the network or adjacent networks by means such as public blockchain records linked to given CIDs, or other technological compatible means. (Which specific blockchain or other system would be appropriate TBD)
  * Apps would also receive collaborative filtering signals from users and third party partners (such as, for example, non-profits or governments), such as reports or flagging of CIDs, which can be added as context in their assessments and resulting actions, and made transparent and accessible to users of the system, or in other public records.
  * Especially for new and small platforms and dapps that might not have the resources to run a full moderation operation of their own, the ability to subscribe to third party assessments and moderation actions might be very useful in early bootstrapping efforts to grow their network and user base.
* Users could choose to take automated filtering actions locally based on the assessments and moderation actions made by the platform or by other trusted third party assessors, and would be able to analyze at any time the assessments made and actions taken by any assessor in the ecosystem.

## Third Party Assessments & Complaints Handling

* Third party assessors would be able to perform similar overlapping functions to the app administrators themselves:
  * Third parties (e.g., a non-profit watchdog countering ethnic violence) would themselves actively scan for problematic content on social networks compliant with Songbird, and would receive reports and collaborative filtering signals from users about problematic CIDs.
  * Third party assessors would make public their assessments (under the framework or public standard of their choosing) related to a given CID, and return results to users and platforms who have subscribed to them as a collaborative filtering source.
  * Where assessments may indicate potential legal issues or other gross ToS violations, third party assessors would be incentivized to collaboratively share their results with the apps or platforms. (Incenitivization system TBD; see below fore more thoughts)
  * Again, third party assessments would be available transparently and publicly at all times as metadata associated with a CID in Songbird-linked systems.  
* Third party complainants, whether with a legal complaint or other (e.g., moral complaints about non-illegal content), would also have parity in the ecosystem, in that their well-formed and apparently good faith complaints (*Note*: a complex topic in itself) received by apps and platforms would themselves be treated as third party assessments. That is, within certain parameters (TBD), complaints by third parties become an additional assessment associated with the CID(s) in question, and become publicly inspectable by ecosystem actors. 

## Claims & Counter-Claims

* Any assessment made by any actor in the system could be challenged or objected to by any other actor in the system, and the challenge would be appended as an additional third party assessment to the CID’s metadata record.
  * Accommodations would need to be made for legal regimes like the DMCA (or perhaps the British defamation system), which have specific requirements for claims and counter-claims. 

## Privacy & Data Protection Considerations

* It is assumed that businesses acting as legitimate hosts of app or platform data will be hosting that data under some form of contractual obligation which will explicitly spell out roles and responsibilities to take, or not take, action in accordance with the instructions of the service contracting them. (e.g., in GDPR parlance, if a given app were considered as a controller, and the host were the processor, then these would be an especially relevant considerations)
  * Under a system of contractual relationships like this, in the event that a host receives a third party complaint about a CID used by an app/platform they are under contract with, the host would likely transmit that complaint to the controller or app/platform to make an assessment, which would append the complaint as a third party assessment to the public record, and transmit back instructions for the host to perform on their behalf. 
    * *Note*: This proposed relationship is similar to how CloudFlare or AWS currently handles complaints received by third parties about content which is hosted by a given web platform customer; they forward or pass-through the received complaint to the responsible platform to take action.
* Assessments need not necessarily be negative (e.g., a third party fact-check that verifies information contained in a CID), and positive assessments by verified sources might be used in algorithmic rankings.
  * However, in the event that assessments could be negative or unwelcome, and potentially affect the rights or reputation of a natural person(s), further consideration must be given to how best to reconcile the necessity of a given public assessment(s) of content associated with personal data, and the protection of persons (e.g., pseudonymization, and other measures), and legal compliance in relevant jurisdictions (e.g., Right to Erasure under GDPR, CCPA, etc.).
    * Further, if assessments were to be linked to a blockchain, investigations would need to be made regarding options for amending or redacting records in appropriate circumstances under relevant data protection law.
    
## Heinous & Illegal Content Concerns

* Where assessments made by third parties (e.g., PhotoDNA for CSAM, or GIFCT for terrorist materials) indicate that a given piece of content is illegal in a given jurisdiction or especially heinous, care must be taken to prevent making public lists of “bad” content available which might be maliciously misused, through protective measures such as double-hashing and other means.

## Incentive Layer For Ensuring Quality Assessments

* An incentive layer should be devised for Songbird, the intent of which would be to actively reward quality content assessments and moderation or filtering actions in line with a given standard(s), and hopefully diminish the likelihood and impact of potential abuses of the system (e.g., such as brigading of assessors with erroneous or malicious reports of content infringements). 
  * The incentive system would also need to be designed to function such that actors who took up the role of assessors within the system would be sufficiently rewarded to create or supplement viable businesses from their assessment and moderation activities. 
  * If these assessments were to be linked to a blockchain, the concept here might be something like “moderators as miners.” For every assessment or moderation action taken which successfully fulfills defined parameters, moderators would receive an appropriate reward.
  * Rewards could be distributed by apps to their users, enabling them to deputize users and trusted third party partners to take mutual responsibility for keeping platforms in good health. 
  * Rewards might also come from foundations or other non-profits which deputize users across many platforms to submit compliant reports within their sphere of interest to the organization for assessment and actioning.
  * Users themselves might also be able to put up bounties or staked coins when they report content to be assessed to third parties, in order to fund that assessment.
  * Additionally, there could be levels of verification for partner providers of assessments and moderation. This could perhaps be similar to the role of Filecoin Notaries, but instead of distributing datacap, they distribute content assessments under a given framework, and reward users under the framework of their choosing for reports they consider “valid.”
  
## Browser Level Considerations

* Since the browser is likely to remain the primary means of interacting with content, it would make sense if the browser was the means through which the user was able to customize their chosen content settings across apps and platforms. It would also make sense if browsers had some sort of embedded functionality for making, sharing (including reporting problematic content), receiving, and subscribing to assessments and moderation actions from collaborative peer-to-peer filters and third party assessors. 
  * If users attempt to visit content which allegedly infringes on their own local content settings, or those of assessors to whom they are subscribed, or those pertinent to their jurisdiction, they might receive an in-browser notification of the alleged infringement, along with additional information. (i.e., part of the browser’s role within Songbird is to make visible the various assessments and moderation actions made by different actors within the ecosystem against a given CID). 

## Additional Reading

* "[Why decentralisation of content moderation might be the best way to protect freedom of expression online](https://www.article19.org/resources/why-decentralisation-of-content-moderation-might-be-the-best-way-to-protect-freedom-of-expression-online/)" by Article 19
* "[Decentralised content moderation](https://martin.kleppmann.com/2021/01/13/decentralised-content-moderation.html)" by Martin Kleppman
* [Moderation in Matrix](https://matrix.org/docs/guides/moderation) by Matrix.org
* [Block Party App](https://www.blockpartyapp.com/): Includes some interesting example local & collaborative filtering functionality for Twitter
