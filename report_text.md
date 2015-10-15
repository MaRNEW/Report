## Report Text
### This Document
This document is a place to collect text for the MaRNEW Workshop Report. __This is not the report itself__, just a place to work on the report text collaboratively.

### Agenda
Thur 24	
* 09:00 – 09:20	Introduction: welcome, introductions and announcements
* 09:20 – 10:00	Scene Setting: defining goals, layouts and key in and out of cope topics.
* 10:00 – 11:15	Session 1: Encryption Deployment Considerations
* 11:15 – 11:45	Coffee Break
* 11:45 – 13:00	Session 2: Trust Models and User Choice (Privacy)
* 13:00 – 14:00	Lunch
* 14:00 – 15:45	Session 3: Sending Data Up for Network Management Benefits
* 15:45 – 16:15	Break
* 16:15 – 17:30	Session 4: Sending Data Down for Network Management Benefits
* 17:30 – 18:00	Day 1 Wrap Up

Fri 25	
* 09:00 – 10:30	Session 5: Application Layer Optimisation, Caching and CDNs
* 10:30 – 11:00	Break
* 11:00 – 12:30	Session 6: Transport Layer: Issues, Optimisation and Solutions
* 12:30 – 13:30	Lunch
* 13:30 – 14:30	Session 7: Technical Analysis and Response to Potential Regulatory Reaction
* 14:30 – 15:30	Parking Lot: time to review open questions from the last two days
* 15:30 – 16:00	Break
* 16:00 – 17:00	Roundup

### Scene Setting: defining goals, layouts and key in and out of cope topics.
* Increasing encryption
* Issue of qualifying trust
* Anti-spam, malware are real problems. Need use cases.
* Transport issues, radio network vs transport? 

#### Scope
* In discussion we should assume: No broken crypto, Ciphertext increasingly common, congestion does need to be controlled as do other transport issues and Network management including efficient use of resources, in RAN and elsewhere, has to work 
  * How/why is RAN different for transport; help us understand the complexities of the RAN and how hard it is to manage and why those matter 
* What are the precise problems caused by more ciphertext 
* Identify players, incl. Users, and resulting tensions and how ciphertext changes those 
* Some solutions will be radically changed by ciphertext, it's ok to talk about that 
* As good as possible Quality of experience for end user is a goal 
* Our aim for the next two days is to analyse the situation and identify specific achievable tasks that could be tackled in the IETF or GSMA (or elsewhere?) and that improve the Internet given the assumptions above 
* We should not delve into: 
  * Ways of doing interception (legal or not), see RFC2804 for why 
  * Unpredictable political actions

### Session 1: Encryption Deployment Considerations
* Gave light to issues and existing solutions
* Document: The Effect of Ubiquitous Encryption
  * increased encryption impact
  * collection of current security and network management function impact
  * Incident monitoring (becoming more difficult)
* Encryption will increase security 
 * but monetary motivation behind selling boxes for preventing security attacks.
* Document: Network management of encrypted traffic
  * Mobile centric document
* Discussion
  * Radio networks are different 
  *  Cell handover creates not modelled in the TCP chain

### Session 2: Trust Models and User Choice (Privacy)
* 64% of users said concerns over privacy have increased
* 67% would like to do more to protect privacy
* Web (and internet) is responding
* Network operator is more like 4th party
Good faith management strategies are indistinguishable from attacks. Bad actors will use those * vectors. 
* Policy controller: consent from one endpoint 
* Consent may be needed from all endpoints
* Discussion 
	* Difficulties finding useful APIs or maintaining policy
* Need finer granularity and more transparency about implications of choice
	* more immediate feedback on costs and benefits
	* authentication is often missing
	
### Session 3: Sending Data Up for Network Management Benefits
* Radio environment is complex, difficult to use with TCP 
* Collaborative frameworks between content providers and mobile operators
	* Mobile Throughput Guidance
* Base station will have a key role. Can a controller adapt, and preserve E2E?
* TCP
	* Fixing TCP may not be the answer to a broken TCP
	* a different Internet: SPUD, ICN?
	* TCP is based on specific network model
	* Need abstractions for making transport protocol evolve
* Up-the-stacks solutions (blind caches)
* Whole network is important
* Avoid personal identifiers
* Content provider motivation to encrypt: avoid in-network modifications

### Session 4: Sending Data Down for Network Management Benefits
* Cooperative traffic management: meaningful capacity sharing, reacting to wireless link layer * conditions, privacy friendly
* TCP feedback to senders and receivers
* Middleboxes treat data differently according to types
* Mobile network manages applications based on the resources available
* 3GPP has defined PCC-QoS mechanism, encryption breaks this:
	* if there is a lack of radio resources, you may release the wrong services
	* during handover can't well adapt services
	* middlebox services stop working
* Does it make sense for apps to send data to networks?  
* Latency vs. bandwidth - preference? Needs incentive framework
* Assumption that applications need to declare the QoS they need: never worked.
	* 1 bit of information, where to do this?
* FQ-codel 

### Session 5: Application Layer Optimisation, Caching and CDNs
* Trusting a fixed network CDN in a mobile context (CDN is content provider)
* CDNi work
* Content providers make assumptions that the network will adhere to standards
	* Costly if that doesn’t happen
	* Adaptive streaming just responds to network situation
* Developers develop on WiFi
* Not every company can build a cache infrastructure 
* Problem Statement: Encryption is not the problem, rather a catalyst to get together to discuss * network management in the broader sense.
* Actors: application provider, network, device. work together!
* Operators work with CDNs and do caching
* Optimisations: way to design the network layer or transport layer?
* Split browsers exist, and are needed now, hopefully go away
* Split browsers exist, and are needed now, hopefully go away
* Keyless SSL
* Blind cache
* Testing and Metrics
	* Standards compliance helps testing
* What’s the one thing you could do if it related to the application layer?
	* metrics to allow for better resource allocation
	* metrics
	* network is calibrated to handle applications best
	* anything that makes it easier for the application to adapt
	* blind cache
	
### Session 6: Transport Layer: Issues, Optimisation and Solutions
* Collaboration essential 
* Bufferbloat is an issue
* Congestion Control innovations
* Problem identification: resource optimisation
* 1 bit: how and where
* Need data and metrics
* Traffic classification, a solution?
* Metadata schemes can be exploited
* ECN

### Parking Lot
* Submitting meaningful data to IETF
* CROWN as a BOF in BA on co-operative resource management
* Layer of Applicability

### Successes
* Know the people
* Understand topics, technologies and issues
* Discussed some good ideas

### Ideas
See [Generated Ideas](https://github.com/MaRNEW/Output_Documents/blob/master/generated_Ideas.md) list. 





	

