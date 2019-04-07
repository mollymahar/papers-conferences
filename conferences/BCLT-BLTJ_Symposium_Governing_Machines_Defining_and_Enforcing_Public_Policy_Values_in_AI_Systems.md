### 23rd Annual BCLT/BTLJ Symposium 
# Governing Machines: Defining and Enforcing Public Policy Values in AI Systems

[Agenda/Website](https://www.law.berkeley.edu/research/bclt/bcltevents/2019bcltbtlj-symposium/agenda/)

This was a fantastic two-day symposium filled mainly with legal and policy experts and scholars, along with a few technical data science folks and some domain experts in healthcare.

We covered many issues relevant to my current work, including: 
- Fairness and bias in algorithms
- The future of work, and what role humans should play in partnership with algorithms (and vice versa)
- Concerns around skill fade and attention when humans and algorithms are working together
- Transparency vs explainability and how the right choice is often context-dependent
- What methods are appropriate for validation and testing of algorithms? 

### Panel: Fairness and/or Privacy & Dignity
- FICO judges models on criteria of: speed, accuracy, explainability, and palatability. ML wins at speed and accuracy, but traditional statistical/existing models win at explainability and palatability.
- When privacy issues arise, be aware that taking that data out of the dataset leads to more bias (unbalanced dataset)
- "I can't imagine any scenario in which more data = fairness. Maybe accuracy, but not fairness." _Meg Leta Jones_
- "Salvation through mechanization" isn't going to happen _Meg Leta Jones_
- "Antagonism can lead to trust" (speaking about how adversarial systems, like the media and our justice system, engender more trust in outcomes than private governance structures at the corporate and industry levels, and how she does not like seeing governments holding hands with industry) _Meg Leta Jones_ 
- If we believe privacy is a fundamental right, we need international standards
- Organizations deploying models are ultimately responsible (read: liable) for fair models, but it isn't always recognized that way. There are liability issues that require documenting how you as an org are using reasonable care when creating and deploying models.

### Panel: Safety & Humans in the Loop
- Reasons for having humans in the loop:
	- collaboration and complementarity of skills (can do more complex tasks together than either can do singularly)
	- discovering blind spots of AI
	- joint executability for reliability
	- Safety, accuracy, fairness, dignity, legitimacy
- Big questions/issues:
	- Latency and handoff time from automated system to human is LONG (attention and focus are difficult)
	- How do you get humans to maintain vigilance over long periods of time when automated system is running?
	- What redundancies do you build between/within systems?
	- Need to avoid false negatives
	- Degradation of skills, "skill fade"
	- How do/can/should humans overcome errors in the automated system (especially in planes or cars, where safety is a major concern?)
- Reality vs. appearance leads to misalignment and undermines our capacity to understand and reason about automated systems (e.g. opportunities for intervention or finding the source of system errors)
	- **Add slide image here**
- Humans have ingenuity and keep finding ways to take themselves out of the loop (e.g. Ebay sells a workaround for the Tesla autopilot which requires human hands on the wheel to ensure you're ready to take over)
- Adding intentional friction to ensure that humans are _actually monitoring_ the system as it runs
- Important for humans to understand the conditions in which they do NOT need to be in the loop (there is often an overreliance on automated systems, especially in the autotonomous vehicle realm)
- Updates to AI models that have humans in the loop don't always match the mental model that users have developed about the system...this is a danger area (e.g. Tesla crashes in autopilot, I'd also argue the Boeing 737 Max 8 MCAS system addition)
- Running simulations can help with data scarcity in reinforcement learning
- We NEED open protocols in AVs (autonomous vehicles) because we want them to talk to each other. Black boxes in airplanes are an example of an open system.
- Future of work and "occupational polarization" into lower skilled jobs, leading to underemployment if not unemployment. But don't fall into technological determinism here. This is a question for us as citizens, what do we want to do about it?
- Equity issues of AVs: they can only operate in areas where they're trained. What about unserved areas?
- Situational awareness of humans is getting more difficult, because machines "sense" things differently (e.g. AVs getting tricked by stickers and thinking something is there when it's not, Alexa hearing sounds that are way outside our auditory range)
- We should start with stark examples, and then move into more subtle examples once we have the stark ones figured out (referring to Trolley problem)

### Panel: Machines of Manipulation
- Tech companies are mendacious, they are hiding things, even from employees. "We might be wrestling a beast we don't understand, and that has fundamentally different values." _Chris Hoofnagle_
- Experiment run by Michael Carl Tschantz around Google ads, setting the user profiles for ad settings to be either male or female and looking at results. Google changed their UI, now he couldn't run that experiment again.
- Need for external testing and validation of these systems. Understand if it can't/shouldn't be the general public (IP concerns are often cited by tech companies) but scholars, civil society and government should have access.
- "Even if tech companies are not _responsible_ [for outcomes], they should be _accountable_" (in terms of needing to explain why/how something happened, not necessarily that they need to accept blame or that blame is even on the table) _Michael Carl Tschantz_
- MCT ran through some interesting analogies, including the idea of the drug-sniffing dog as the original "black box" algorithm.
- CFAA [Computer Fraud and Abuse Act] needs to account better for outside testing of systems. Currently some researchers are worried about or refrain from certain testing because they fear consequences.

### Keynote: Deputy Commissioner of the Singapore Personal Data Protection Commission
- Argues that we do not need new policy for AI, because we already have existing frameworks that cover the issues we're worried about:
	- For the company:
		- Contractual liability for services
		- (Vicarious) responsibility for decisions
		- Consumer protection considerations
	- For the AI engine:
		- 3rd party software license
		- Algorithmic transparency or explainability
		- Benefitting from algorithmic audits (regulator or consumer?)
	- For the data source:
		- When is data personal?
		- Who is the data controller?
		- Consent and purpose limitation
- Introduced the idea of Human-Over-the-Loop in addition to human-in-the-loop and out-of-the-loop, which I liked. Human-Over-the-Loop adjusts parameters _during_ the execution of the algorithm (ex of Google Maps navigation, as a user I can change course while it's running and the system adjusts to the new route)
- **add risk analysis slide about how to choose where human goes in the loop**
- Singapore has a governance framework available online [here](http://www.pdpc.gov.sg/model-ai-gov)

### Panel: Ethical Machines – Professional Knowledge and Ethics
- Really interesting talk about the role of ML in healthcare and legal professions (as regulated professions)
- FDA regulates both software IN a medical device, and software AS a medical device
- What should the FDA do about the _learning_ aspect of ML? It's typical to have a closed/locked model in production rather than an open one, but the rates at which software learn and improve are much faster than the typical medical device production periods, so regulating these updates will tax the system.
- Tension exists between controllers (regulators, payers, app gatekeepers like App Store) and innovators (researchers and industry)
- American Medical Assoc. calls AI "Augmented Intelligence" because they want practitioners to work WITH the AI. I really like this terminology!
- ML trains on the _outcomes_ of human decisions, rather than the train of thought or decisions themselves. Leaves it open to so many problems:
	- assumptions and optimizations
	- operationalizing the target variable (construct validation is relevant here)
	- choice of model
	- thresholds
	- training data
- These algorithms are acquired as *procurement* but they are functioning as *policy* choices
- Contestability can be a governance structure
- Lots of litigation is happening around self-service legal services, and the definition of "what is the practice of law?" and where the boundaries are
- These systems mean that lawyers are handing off judgment early on in the process, and then the models are not iterable.
- What's the structure for deciding whether to tolerate false negatives or false positives?
- "Lack of shared language is a huge problem" in creating these _diverse_ teams, because everyone comes at it with a different understanding. _Pilar Ossorio_ 

### Lecture: Andrea Jelinek, Chair of the European Data Protection Board
- More guidelines and opinions for consistent application of GDPR are coming
- EU will continue to try to drive movement in addressing AI regulations

### Panel: Trust but Verify – Validating and Defending Against Machine Decisions
- Google presented a great deck about how they try to be "accountable to people" through Explainability, Interpretability, and Testing/Validation:
	- Explainability aims at non-technical audiences. Dependent on how consequential, how much trust already exists for the product, how opaque the system is, potential legislation, how new or novel the system is, how contestable it is, and how much agency users have to contest it.
	- Interpretability aims at technical users. Includes tools to explore datasets for inclusion (e.g. What If tool), tools to debug models for inclusion, and Model Cards for Model Reporting.
	- Testing/Validation aims at their internal Red Team testing from a fairness and ethical perspective.
- The idea of transparency or explainability is context-dependent (this from Helen Nissenbaum). "I need to know how my refrigerator works" can mean either _How do I adjust the temperature, or the shelving?_ if you're a customer, or _I need to know how to troubleshoot this, and need lots of details_ for a repair worker.
- For some purposes, we simply **should not use models and systems for which we cannot explain why we got the answer**. 
- Testability can mean internal, external and aligned, or external and adversarial. At the policy level, _we need external and adversarial testing_.
- We haven't talked enough about use cases and scenarios for these systems. Some are designed for legitimate/common purposes (e.g. ethical or societal), and some are created as zero-sum systems (e.g. price discrimination, housing choices, etc where two parties are at odds with each other).
- Contestability allows for dispute." If you can challenge something, you may be able to change it." _Jennifer Urban_ Downside of contestability is that it's a _post-hoc detriment_, the harm has already happened.
- **Add slide with requirements for meaningful contestation**
- Judicial opinions offer a really good model of explainability.
- Slovenia has an approach whereby disparate impacts from algorithms are explicitly prohibited without an explicit law authorizing that particular usage.
- To say that we have "solved fairness" is impossible—-it's not just a bug that can be closed. It's ongoing. _Jennifer Urban_
- "I don't buy this _don't regulate too early_ argument. There will always be people who can innovate. Otherwise it's a race to the bottom." _Helen Nissenbaum_ I love this because it's similar to how designers think. We have to work within constraints. Regulation is just a constraint. It leads to creativity.
- We need "infrastructuring" here--shared language, concepts, and processes. _Deirdre Mulligan_
