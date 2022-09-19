# Polkadot Fellowship Manifesto

Version 0.1

Ranked, compensating membership organisation for vote-casting.

## Goals

- Compensate all members and incentivise their continuation in ecosystem.
- Rank those with core development expertise and experience, where a higher rank reasonably implies a greater level of expertise in Polkadot/Substrate technology and value within that ecosystem.
- Primarily, this covers expertise/value concerning:
    - Polkadot core protocol (including parachains, XCMP, HRMP/DMP/UMP, BABE, GRANDPA and cryptographic datastructures specific to Polkadot);
    - Polkadot node implementation (including peer networking protocols, topology strategies, sync strategies, internals of complete node implementations);
    - Polkadot runtime (including Frame internals, runtime/host APIs, pallets utilised by Polkadot & its system chains and XCM)
- Secondarily, this coveres expertise/value concerning:
    - GRANDPA-based bridges, common-good chains and pallets utilised by them.

### Non-Goals and Limitations

This collective is *discipline specific*: It covers the domain of *protocol engineering and development* only. It is not intended to recognise nor incentivize activity of other fields, however related including, but not limited to, recruitment, management, education, outreach, mentorship and research. It is expected that there will be additional "fellowships" for such disciplines in the future.

## Summary

A membership-oriented governance body inspired by expertise-based structures such as the [ITF](https://en.wikipedia.org/wiki/International_Taekwon-Do_Federation). Requires its own pallet/set of pallets, which enforce the rules of ranking and membership.

## Rules of the Fellowship

1. Act in the interest of Polkadot.
2. Respect the philosophy and principles of Polkadot.
3. Respect the operational procedures of the Fellowship, including voting in line with the Mechanisms and Specifications.
4. Respect your fellow Members and the wider community.

Breach of the rules, especially rule #1, leads to demotion or expulsion via referendum.

## Promotion Mechanism

Steady-state rules are stated below. During the initial bootstrap phase, timelines may be shortened to expediate decentralisation.

Any account may register as a *Candidate* for a basic deposit. They have rank 0.

A Member may Apply For Membership of a Candidate to become a *I Dan Member*.
- With a one month voting period, all Fellows (Members of at least III Dan) are invited to rank-vote for or against the Membership. There must be a majority of votes in favour.
- Voting is quantitative as well as qualitative and precedent of I Dan Members should be taken into account when making the decision of whether Membership should be granted.

A Member may Apply for Promotion to have their Rank incremented by one. This is subject to Promotion rules:
- With a one month voting period, all Members who rank at least two grades more senior than their promotion rank (saturating at Rank 9) are invited to rank-vote for or against the Promotion. There must be a majority of votes in favour.
- Voting is expected to follow the Rank Specifications. This takes into account:
    - Whether contributions are at a quality and insight level equal or greater to that of peers from the promoted Rank.
    - Whether their past contributions have, in hindsight, been of lasting value.
    - Whether they are persistently and consistently making themselves available for the support of the network.
        - For Rank 4 and above, a proven availability is required with the Member minimising periods of abject unavailability and making these periods clear to the Fellowship ahead of time.
    - Whether they have a voting record broadly in accordance with higher ranks.
        - For Fellows and Architects, Membership votes where there is unanimity among those of higher rank should generally agree with that consensus for 95% or more of the historical voting record.
        - For Members of Ranks 1-6, there is a minimum voting activity level, starting at 90% of all votes eligible and reducing monotonically to 40%.

Ranks are generally kept regardless of current focus, however members who feel they are not contributing actively for more than two months at a time are expected to voluntarily place themselves on a passive allowance.

Once over a period of time (three months for members below the rank of Fellow, six months for non-Master members who are Fellows or beyond) are automatically demoted unless their rank is re-approved by their peers. This upvote is similar to a grading and they should submit clear and concise evidence showing they are retaining the qualities expected of a member of their rank and have been contributing substantially for the period of time they have been on standard allowance.

There is no concept of suspension. Members are expected to be able to defend their rank every 3/6 months. The price for effectively suspending one's role (assuming one is not a Master) is a slow demotion through the ranks.

Master ranks are the exception: once a Master, one generally remains a Master regardless of occupation or knowledge. The only way a Master may be demoted or lose their rank entirely is through being found to have acted contrary to Polkadot's interests through a general Polkadot referendum.

### Notes

All voting is expected to follow the Promotion Mechanism and Rank Specifications; disregarding these should be taken into account at the Fellow's subsequent promotion(s) and evaluation(s).

Ideally, all voting is commit-reveal. However in the interests of expediance an initial implementation may be public.

### Rank Voting

Voting generally happens through cumulative Rank-Voting. This simply means that Members votes are weighted by their Rank as an item in the geometric series. Rank 1 would have a weight of 1, rank 2 would have a weight of 3, rank 3 a weight of 6, &c.

For Membership/Promotion/Continuation Votes, a particular Rank is required for voting.

## Rank Summary

| Dan Rank | Name            | Grouping   | Quality      | From I Dan | Material     | Hardness  | Activity |
| -------- | --------------- | ---------- | ------------ | ---------- | ------------ | --------- | -------- |
| n/a      | Candidate       | n/a        | n/a          | n/a        | (White)      | n/a       | n/a      |
| I        | Humble          | Members    | Proficiency  | n/a        | Graphite     | 1-3 Moh   | 90%      |
| II       | Proficient      | Members    | Prof/Buidl   | ~1 years   | Stibnite     | 2 Moh     | 80%      |
| III      | Fellow          | Fellows    | Building     | ~2 years   | Galena       | ~2.5 Moh  | 70%      |
| IV       | Architect       | Architects | Buidl,Design | >3 years   | Obsidian     | 5-6 Moh   | 60%      |
| V        | Architect Adept | Architects | Design,Buidl | >4 years   | Ilvaite      | 5.5-6 Moh | 50%      |
| VI       | Grand Architect | Architects | Design       | >5 years   | Magnetite    | 5.5-6 Moh | 40%      |
| VII      | Free Master     | Masters    | Commitment   | >6 years!  | Black Spinel | 8 Moh     | n/a      |
| VIII     | Master Constant | Masters    | Commitment   | >11 years! | Carborundum  | 9 Moh     | n/a      |
| IX       | Grand Master    | Masters    | Commitment   | >19 years! | Carbandos    | 10 Moh    | n/a      |

## Rank Specifications

### Rank 0 ("White belt"): Candidate

This is the beginning rank and indicates someone new to the Polkadot protocol and codebases, but who have taken a first concrete step through placing a membership deposit and finding a sponsor.

Candidates may be of many levels prior to promotion to rank 1 and through a secondary system these levels may even be codified and properly recognised on-chain.

### `I Dan`: Humble Member

Approx. academic analogue: **Foundation course**
Material: **Graphite** _(1-3 Moh)_

![Graphite](https://www.thepearlsource.com/blog/wp-content/uploads/2021/12/graphite-black-gemstones.jpg)

The (potentially) softest of the materials, symbolising the beginning of the journey and the most to learn from the world. Also shares the exact same chemical composition as the material of the highest rank Grand Master - the hardest material - symbolising the individual's potential to go all the way.

The primary qualities which should be present and clear in those being given the rank are aspiration, knowledge-discovery, knowledge-sharing and active maintenance. They should demonstrate commitment to the protocol's development through mastery of at least one major component as well as having a broad understanding across the protocol. They will demonstrate commitment to pooling and sharing protocol knowledge through establishing a pattern of availability or communication in one or more online media; forums, chatrooms, issue trackers or Q&A sites. A pattern of general availability on synchronous communication media would also count in the individual's favour and demonstrate a commitment to the network maintenance. The candidate should have a rudimentry awareness of, and ability to be educated on, overall priorities and tradeoffs in development & design of a global, decentralised and unstoppable network, including centralisation risks, non-jurisdictionality, privacy, automation & maintenance vs autonomisation & ownerlessness.

The Candidate must clearly demonstrate an independence of mind and spirit. They should be able to work alone and without direction, to investigate and problem-solve without need for assistance and to be responsible for the design, implementation and/or continued maintenance of a Polkadot component or sub-system which could reasonably be considered important for the continued health and operation of the Polkadot network. The Candidate should have made three clear demonstrations of protocol expertise. Possible examples of this may be: identifying and fixing a non-trivial protocol issue; being available and playing a crucial operational role for a network fix; proposing a reasonable and non-trivial protocol innovation; or doing a valuable, innovative and insightful refactoring or alteration.

There is no specific time which must have passed with Polkadot being the individual's primary life-focus prior to attaining this rank, though a reasonable expectation would be that they have been working on core Polkadot technology continuously for around 12 months.

#### Requirements
- Primarily designed and implemented a minor or auxilliary component.
- Should be able to list all key goals/principles/tenets of project philosophy and how these relate to technology.

### `II Dan`: Proficient Member

Approx. academic analogue: **Bachelor's degree**
Material: **Stibnite** _(2 Moh)_

![Stibnite](https://www.thepearlsource.com/blog/wp-content/uploads/2021/12/stibnite-black-crystal.jpg)

As a key component in many pyrotechnic preparations, Stibnite represents the process of transformation, symbolising rebirth and metamorphosis. It symbolises the transformative nature of the journey of the individual on the way to becoming proficient and the need to change ones perception as the understanding of the protocol evolves.

A member at this rank should be a core part of the team. Clear demonstration of knowledge of the protocol is crucial, but since the individual knowledge of the protocol is unlikely to be complete then general knowledge acquisition and communication/sharing is also very important. The individual should be becoming deeply familiar with at least one major area of the protocol in their role as a builder and should be becoming increasingly familiar with design considerations typical in protocol development. They should not be asking dumb questions and should instead be making reasonable suggestions. They should be demonstrating a readiness to be a network maintainer through increased levels of availability. Excellent candidates will already be "on-call" for the components of which they have a deep understanding.

It is generally expected that the participant will have been practicing Polkadot as their primary life-focus for at least **one** year, unbroken, after attaining the previous rank.

#### Requirements
- Usefully assisted in implementing a major component from start to finish.
- At least one published long-form semi-technical article concerning Polkadot.

### `III Dan`: Fellow

Approx. academic analogue: **Master's degree**
Material: **Galena** _(2.5-2.75 Moh)_

![Galena](https://www.thepearlsource.com/blog/wp-content/uploads/2021/12/galena-black-gemstones.jpg)

Galena is the mineral form of lead. This was known, mined, refined and used by the ancients, and its long role serving human-kind symbolises the foundational level the individual has now reached by completing the first third of the ranks, and also serves a reminder that recognition of skill and commitment is provisioned on the individual's continued servitude to the whole. As a Fellow, the individual attains new privileges and the heavy nature of the substance represents a need of the individual to act with due consideration on decisions which their new responsibility brings.

As a foundational grade, a Fellow represents both a ceiling and a floor: becoming a Fellow indicates the individual has enough knowledge and skill to build substantial protocol components (i.e. all but the major protocol components, e.g. a pallet or 2-10,000 line crate) alone and with high expectations that they will be completed correctly and to a high standard. They should be able and willing to support that which they built given that it is running 24/7 on a public network. This means a commitment to availability even when it may be inconvenient for them and, in periods of lesser-availability, taking on a responsibility to make this clear to their team prior.

As a Fellow the individual, in some quite real sense, represents the Polkadot Network and as such must be ready and willing to both defend it and its values. They should not merely adhere to the basic community code of conduct, but to hold themselves to a higher standard, maintaining a high level of calm and humility but also honesty and directness. They have a responsibility to represent the Fellowship as well as the network and this should be done in a polite and non-cambatitive, but also honest and forthright fashion. Internally, they should be both helpful, tactful and well-spirited, understanding that Polkdaot is a team effort.

A Fellow must have a comprehensive knowledge of the overall priorities and tradeoffs in the development and design of a global, decentralised and unstoppable network and be able to express and explain themselves on these matters confidently.

It is generally expected that the participant will have been practicing Polkadot as their primary life-focus for at least **one** year, unbroken, after attaining the previous rank.

#### Requirements
- **In-person grading.**
- Defense should include a chat on the philosophic principles and their relation to the technology where they demonstrate expert knowledge confidently and betray no misinterpretations.
- At least three published long-form semi-technical articles concerning Polkadot.
- Played a primary role in implementing a major component from start to finish.
- At least one ecosystem presentation on Polkadot or some component of it.

### `IV Dan`: Architect

Approx. academic analogue: **Doctorate**
Material: **Obsidian** _(5-6 Moh)_

![Obsidian](https://www.thepearlsource.com/blog/wp-content/uploads/2021/12/obsidian-black-stones.jpg)

This is the first of the middle three *Architect* ranks and connect the portion of the journey where the individual develops beyond knowledge on the past and is expected to contribute to core innovations and design of the protocol's future. The next three materials symbolise three qualities required of the individual during their journey of become a protocol Architect.

The materials are all of approximately the same hardness symbolising that all three qualities are of comparable importance, and their hardnesses (5-6 Moh on each) sit in between the softer materials of the lower three ranks and the harder materials of the upper three ranks, symbolising the maturing nature of the architect's intellect.

The first, for the grade of 4th Dan is Obsidian. It is essentially volcanic glass, composed of silicon with other light elements and easily forms sharp edges. It has been used in tools since ancient times especially for creating cutting blades. The sharp blade symbolises the single-minded focus required by the individual in both becoming a subject matter expert and in inovation itself. It is very slightly softer than the other materials of the expert ranks reflecting that a deep level of expertise, while very important, is the junior of the three qualities.

To attain this grade the candidate should be demonstrating a shift in their focus from the attainment of specific knowledge, comprehension and skills to the less knowledge-based and more creative elements of protocol development: design, invention, innovation and architecture. Rather than (just) plentiful incremental low-level improvements to the protocol, substantial valuable individual contributions to the (r)evolution of the protocol should have been demonstrated through the design, architecture and/or implementation of key future components which were (ultimately) found valuable by the Fellowship. Rather than comprehension, their ability to experiment, design and build new technology must be beyond question and their truly novel ideas and designs must be of a consistently high quality and at least occasionally beyond the imaginations of those with higher rank.

The participant will have been practicing Polkadot as their primary life-focus for at least **one** year, unbroken, after attaining the previous rank. However, this is only a bare minimum and should not be taken as a presupposition of the expected amount of time required. The candidate should be only be promoted to this grade once the time limit is over *and* they have demonstrated the appropriate aptitude.

#### Requirements
- Usefully assisted as part of the design of a major component.
- At least one non-ecosystem, non-private presentation on Polkadot. Would typically be industry-wide or academic.

### `V Dan`: Architect Adept

Approx. academic analogue: **Research Fellow**
Material: **Ilvaite** _(5.5-6 Moh)_

![Ilvaite](https://www.thepearlsource.com/blog/wp-content/uploads/2021/12/ilvaite-dark-gems.jpg)

The second material in the middle three ranks is Ilvaite, a mineral which exhibits pleochroism, meaning it appears to change colors depending on the angle in which is it viewed. As the second material in the Architect ranks, it symbolises the need for multiple perspectives, reflecting that great architects often draw upon knowledge and understanding from different teams, areas or even disciplines in order to create a final solution. It should remind the individual that while myopia and deep focus can be an alluring path and even necessary in the pursuit of perfection, they should not overlook the possibility the an alternate form of the problem is already solved by others or that inspiration may arise from apparently unrelated areas of human-pursuits (consider Feynman's story that physics Nobel-prize winning work arose from studying the dynamics of a tea-saucer when spinning in the air).

To attain this rank, the candidate must have demonstrated clear levels of architecture. Their abilities as a builder should now be beyond question and as a leader in technology design should now be becoming clear. They should begin to understand the protocol as a living organism and be able to visualise its path. They should only very rarely misunderstand a protocol consideration, and have a clear grounding in all fields related to protocol design including game theory, economics, programming languages, complexity, enntropy and distributed systems. They should be able to speak with technical authority on all levels of the Polkadot protocol past, present and future.

The participant will have been practicing Polkadot as their primary life-focus for at least **one** year, unbroken, after attaining the previous rank. However, this is only a bare minimum and should not be taken as a presupposition of the expected amount of time required. The candidate should be only be promoted to this grade once the time limit is over *and* they have demonstrated the appropriate aptitude.

#### Requirements
- Play a primary/sole role in designing *and* implemented a major component.
- Usefully assisted in devising ("creating", "inventing", "incepting") a major component.
- At least one published long-form article about technology relevant to but not specifically concerning Polkadot.

### `VI Dan`: Grand Architect

Approx. academic analogue: **Associate Professor**
Material: **Magnetite** _(5.5-6 Moh)_

![Magnetite](https://www.thepearlsource.com/blog/wp-content/uploads/2021/12/magnetite-dark-gemstones.jpg)

Magnetite is a primary form of iron ore. It is ferrimagnetic and both attracted to magnets and able to be magnetised itself. It was used by ancient civilisations in the discovery of magnetism which lead to the use of compasses, and occurs in biological cells used as a navigation aid (with birds and bacteria being two important examples). This material concludes the three key elements of architecture and represents the need not just for the ability to focus on an individual technical direction, nor also to take ideas from broad range of perspectives but also, crucially, to retain a long-term strategic product direction or risk being pulled off-course.

This grade is the highest rank to be arrived at through purely technical prowess and to attain it, the individual must demonstrate they can match or better others of this rank in their absolute technical ability. As a benchmark, they must have played an advisory role in the architecture, design and implementation of at least five major protocol components and actively designed and built at least two from start to finish. They must have demonstrated beyond doubt the ability to nurture into greatness not only new Fellows but also new Architects. They must also be able to withstand or manage the rigours of being a technical architect. A willingness to delegate, to work at a tenable speed and an overall knowledge ones own limitations is crucial.

The participant will have been practicing Polkadot as their primary life-focus for at least **one** year, unbroken, after attaining the previous rank. However, this is only a bare minimum and should not be taken as a presupposition of the expected amount of time required. The candidate should be only be promoted to this grade once the time limit is over *and* they have demonstrated the appropriate aptitude.

#### Requirements

- *Devised*, lead the *design* and overseen (or lead) the implementation of a major protocol innovation.
- At least three published long-form articles about technology relevant to but not specifically concerning Polkadot.
- Discuss: What have you learnt from this individual which you might ultimately find useful in your efforts to help Polkadot succeed?

Note: This is the first rank for which pre-specified discussion points become a crucial part of the grading and where those voting on the promotion must make a qualitative assessment on the outcome of the discussion in comparison to the precedent of prior promotions.

### `VII Dan`: Free Master

Approx. academic analogue: **Professor**
Material: **Black Spinel** _(8 Moh)_

![Black Spinel](https://www.thepearlsource.com/blog/wp-content/uploads/2021/12/spinel-black-crystals.jpg)

As the only named material here which is rarely black (Spinel is commonly one of several other colours), it symbolises the individual's journey through many shades of life and arrival into the set of Masters. As a material far harder than all those previously, it symbolises that the individual's journey as a student is ending and the beginning of their journey as a protector and leader. 

The rank of Master indicates a move into the upper three ranks of the Fellowship and with it a refocusing from the predominantly technical qualities surrounding invention, design, architecture and development into the more philosophic, strategic, socio-political and sophist qualities associated with good leadership. To attain this rank there must have been a clear demonstration of these qualities.

The rank calls for intellectual conversation no longer focussed primarily inside the protocol but also outside into the wider industry and social, political, commercial and technological environment in which Polkadot ultimately sits. Education and advocacy, both at the technical and less-technical levels. This can take many forms, not least written articles, interviews, social media, conferences and other pod/vid casts. At this rank, the individual might reasonably spend their effort split equally three ways: today (expertise and availability on the protocol which is running the network right now), tomorrow (helping design and evolve the protocol which it will become) and the future (helping shape the overall direction of the protocol and including its social and political elements).

Masters are expected to gain themselves (and by extension Polkadot) a good standing and reputation beyond the Polkadot ecosystem. They are expected to be a living advertisement of Polkadot's tenets and its philosophical and intellectual rigour. At this rank they are an outward intellectual representative of Polkadot and must at all times conduct themselves in concordance with both the edge and the humility that a true master of an art must possess.

Masters need no longer defend their place in the Fellowship. However, promotion to Master cannot be done by other members of the Fellowship, no matter the rank. Instead, Masters can only be conveyed by a Root call, generally requiring both the approval of the Fellowship as well as of the network itself through a general referendum. Conversely, it is only through a general referendum that the rank may be revoked.

To attain this rank, the individual **must** have been practicing Polkadot as their primary life-focus for **six** years in total, in addition to the demonstrating the administrative, knowledge, intellectual, social and skill-based qualities expected.

#### Requirements
- Contributed to the broader understanding of the philosophy behind Polkadot during an in-depth conversation. Perhaps through drawing parellels to existing body of literature, perhaps through rational discourse with experts. Should be ready and confident in their ability to explain and defend the newfound understanding.
- Several major presentations on the Polkadot network and protocol with an audience that included peers from other ecosystems and/or industries.
- Discuss: Does the wider academic community or industry tend to learn from this individual (even if the individual did not discover this knowledge themselves)?

### `VIII Dan`: Master Constant

Approx. academic analogue: **Professor in a historical seat**
Material: **Carborundum** _(9 Moh)_

![Carborundum](https://www.thepearlsource.com/blog/wp-content/uploads/2021/12/carborundum-black-gems.jpg)

Man-made crystal from 1800s, used for cutting & polishing.

As the only purely man-made associated material, Carborundum represents the fact that the Fellowship and their members are forged by mankind, not born of nature. Carborundum, being among the hardest of minerals, finds a lot of use for cutting and polishing; this symbolises the individual's role, changing to that of helping others become polished masters in their own right.

This rank indicates a Master with an elevated level of commitment to furthering the interests of the Polkadot network. To attain the rank, it should be clear that the individual is helping shape the future of the network, its protocol and its overall ecosystem in a way commensurate with the overarching tenets laid out in the Polkadot Paper, the goals of Web3 and the principles of enlightened liberalism.

To attain this rank, the individual **must** have been practicing Polkadot as their primary life-focus for **eleven** years, as well as fulfilling the social and administrative qualities expected of being in the previous rank.

#### Requirements
- At least one article considered canonical by masters which further develops the understanding of the philosophical principles underpinning Polkadot.
- At least one article about an innovation relevant to but not specifically concerning Polkadot which is ultimately recognised as a pan-industry innovation.
- Generally recognised as an intellectual heavyweight outside of the Polkadot ecosystem.
- Discuss: How did this individual's idea or invention become adopted in the wider academic community or industry?

### `IX Dan`: Grand Master

Approx. academic analogue: **Nobel/Field's Laureate**.
Material: **Carbonado** _(10 Moh)_

![Carbonado](https://www.thepearlsource.com/blog/wp-content/uploads/2021/12/diamond-black-gemstones.jpg)

Carbonado is a black form of diamond and the hardest mineral known to man. This symbolises both the peak of seniority and knowledge that the rank represents but also the limitation of human-knowledge and that the journey of discovery never ends.

To attain this rank, the individual **must** have been practicing Polkadot as their primary life-focus for **nineteen** years, as well as fulfilling the social and administrative qualities expected of being in the previous rank.

#### Requirements
- Generally recognised as a philosophical, social, artistic, political and/or technological heavyweight outside of blockchain or crypto.
- Discuss: what outstanding service did the individual provide to the Polkadot network?

## Notes on Master Ranks

The three Dan ranks of Master have a series of sub-ranks (which also function as honours) not recognised within the on-chain voting system and unimportant for voting weight, defined primarily to recognise some exceptional service of the individual to Polkadot. In addition to recognition of effort, they help mark and celebrate milestones within the journey of personal development during which, especially at the stage of Master, time can flow a little too easily with significant events being less apparent.

The Master may reasonably be described by the mainline grouping (Master), mainline rank (Free Master, Master Constant, Grand Master) or specific sub-rank. The latter would be considered most polite since it implies the most knowledge concerning the individual.

Initially no such sub-ranks are defined, but each *Master* shall be free to name one in their new rank as they attain the ranks of `VII Dan`, `VIII Dan` or `IX Dan`.

At most twelve shall ultimately be given for `VII Dan` and sixteen for `VIII Dan`. There is no limit to the number of sub-ranks for those of rank `IX Dan`.

The elevation within sub-ranks must be agreed in-person at a Masters' meeting, and must be for some specific act of special service of Polkadot going beyond the general expectations of contribution at the rank. In general, a sub-rank may be attained no less than six months following the previous, 12 months for sub-ranks of `IX Dan`. Attaining all sub-ranks should be considered strictly necessary for promotion from their rank, however it would be a near inescapable indication that the member should be promoted.

### Obligations of Masters

Being a master comes with additional obligations:
- Fellowship can, through a standard vote of Fellows, implore a Master to assist with some piece of technical work.
- Assistance may be substantial (including advising on strategy, architecture, design, APIs and algorithms) but must be constrained.
- This mechanism is used only in the most extreme circumstances where:
    - Existing non-Master Members are unable to complete the work themselves to a standard needed for network safety;
    - The Master has expert knowledge and can lend knowledge and experience which are crucial to achieve success and otherwise unavailable;
    - The assistance involved is of a clearly constrained scope; 1-2 hours should be the typical expectation in terms of time, though under extreme circumstances, 1-2 days may be needed. Two weeks' of assistance should be considered an upper limit.
- Failure to assist the Fellowship can be considered grounds for breach of Rule #1 and may be considered grounds for demotion or, in extreme circumstances, expulsion. As with all Master-level punishment, this is determined & enforced through General Referendum.

### Annexes, Clarifications and Conventions

On elevation to a Master rank, the individual is able to propose an annex (additional rule), clarification or non-binding convention to this manifesto. Pre-existing rules always take precedence. These ammendments are included by default after a one month challenge period passes, during which time a majority ranked-vote of the Fellows (and above) may cancel it. Ammendments must not break the principles nor any pre-existing rules.

## Allowances

These are a monthly affordance, paid in DOT. There are two levels: standard and passive. Standard should be between the 80th-90th percentile of gross income in the OECD group of countries. Passive is no greater than 50% of standard. The total amount given as passive allowance should be no greater than 10% of the total amount given as standard allowance.

Members are free to place themselves on a passive allowance if they believe they are unlikely to contribute substantially within any given month. (At challenge or grading time, members who do not may find the lack of productivity difficult to explain.) Regardless, members must keep their knowledge and skills up to date.

## Prizes

Since sub-ranks are not available to Members, Members, and especially Masters, are invited to create *honourable prizes*. Prizes should include some sort of endowment (e.g. a DOT gilt or high quality staked DOT derivative) and a description of what it should be awarded for and who should judge. A reasonable selection would be a Masters level vote, but need not be.

Prizes should eventually be recorded on-chain but an initial implementation may not.

## Events and Gatherings

At least once per year the members of the fellowship should gather. This should be paid for by the treasury. Lower gradings (I-III Dan) should happen here (though I and II Dan may happen remotely).

Additional meetings for Fellows and (eventually) Masters. Information on these meetings should (for security purposes) be kept on a need-to-know basis. Disregarding this is a breach of Fellowship rules. Upper gradings (IV-VI Dan) should happen here.

# Appendix

## Terminology

- "Primarily" means vast majority of work done by the individual and if no others contributed then a perhaps lesser but still correct and useful artefact would be delivered.

## Philosophy & Principles of Polkadot

### Enlightened Liberalism

Honesty and freedom. But respect, politeness and tolerance. Required reading:

- The Open Society and its Enemies

### Critical Rationalism

Judge only by actions, not suppositions, associations or words. Required reading:

- A Pocket Popper

### Web3

Reduce the need for the individual to trust the group by providing them with tools to interact usefully with the world themselves. Required reading:

- What Web3.0 looks like

### Polkadot

Decentralised, empower the individual

## Developer Expectations at Rank

APIs/code design:
- Indicatation against Candidacy/Membership: Contributes to noise or stays silent and doesn't learn.
- Indication against Membership: Rarely makes any suggestions, asks questions whose answers are otherwise difficult to discover.
- I Dan: Sometimes makes reasonable suggestions for APIs, rarely makes bad suggestions.
- II Dan: Generally makes reasonable suggestions for APIs, rarely makes bad suggestions.
- III Dan: Sometimes able to identify flaws in APIs of peers or better.
- IV Dan: Generally able to identify flaws in APIs of peers of better.
- V Dan: Occasionally innovative in API design, adapting/importing/inventing ideas that lead to effective solutions.
- VI Dan: Often innovative in API design.

Key aspects when judging code contribution
- Correctness: Does the code actually do what it is meant to do?
- Quantity: How much relevant functionality is delivered in the code?
- Modularity: Is the code only relevant for the immediate features, or was it architected and implemented sufficiently modularly, generally and with sufficient functional-independence to allow for reuse, maintenance and eventual externalisation?
- Quality: Is the code minimal, elegant and comprehensible?
- Timeliness: Was the functionality delivered at the optimum time for maximum value to be extracted through its existence?

Key aspects when judging behaviour:
- The ability to listen and comprehend and form an effective dialectic.
- To avoid ego and the heat & waste brought by pointless argumentation or repeatedly pushing against an answered point.
- Not to be afraid of quietly and succinctly challenging others when to do so would lead to them havng a greater understanding of the world.

## Meta-notes

Careful, now!
- Rank & hierarchy come with baggage.
- Members should know and practice equality and humility.
- Correctness is not determined by rank but nature herself and members must never forget this.
- There could be some requirement to keep on building (at least a minor amount) all the way up to the top in order to keep progressing through the grades.
- Re-emphasise that plentiful teaching, education and rational advocacy is a crucial part of moving through the last half of the grades.

## Ideas & Considerations

- Introducing shadowing a pre-existing Fellow as a requirement for Fellow grading.
- Introduce sponsors:
  - A sponsor is required for each candidate or member who seeks a promotion.
  - The sponsor must be a member of at least two ranks greater than the rank sought for promotion.
  - If a promotion is denied, the sponsor may not sponsor further promotions for a period of six months.
- Require also a small write-up of lessons learned at each grade, especially following the shadowing.
- Master ranks should be encouraged to develop into disciplines separate to Polkadot and find ways to contribute their learnings back into the whole.
- In general, gradings should be conducted in-person. From III Dan grading and above, they **MUST** be in-person unless environmental conditions make it impossible (e.g. pandemic). If the individual wishes to remain anonymous, a mask or other facial-covering may be worn.
- Bring in smaller milestones e.g. public technical presentation.
- Bring in knowledge of principles. Enlightened liberalism, critical rationalism, Web3 & truth vs trust, Polkadot and its 5 guiding tenets in the paper. Candidates should move from basic knowledge to the ability to converse to eventually having a deep understanding and contributing back.
