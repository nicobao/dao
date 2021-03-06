# My opinions on governance for a DAO

How should you organize governance for your DAO to motivate your community towards the goal of your DAO?

## Inspirations

Open-Source/Free Software development in general.
In many ways it relates to DAO. People who don’t know each other come together to build towards a common goal. My inspirations are especially:

- primarily my #1 inspiration is [Pieter Hintjens](https://en.wikipedia.org/wiki/Pieter_Hintjens) lifework in general, his [blog](http://hintjens.com/), his [Social Architecture](https://hintjens.gitbooks.io/social-architecture/content/) book, the [ZeroMQ guide](https://zguide.zeromq.org/doc) and [C4](https://hintjens.gitbooks.io/social-architecture/content/chapter4.html).
- [Everything You Need To Know to Grow Open Source by Dan Allen - lead developer of asciidoctor](https://www.youtube.com/watch?v=a_vqg-go8XI)
- [the Conway’s law](https://en.wikipedia.org/wiki/Conway%27s_law)
- my short experience contributing to various open-source projects. I had for example a nice experience contributing to RedHat's codebase, but I also have had bad experiences which taught me what not to do
- my professional experiences in various style of organizations
- [The Cathedral and The Bazaar](https://en.wikipedia.org/wiki/The_Cathedral_and_the_Bazaar)
- [Stephane Klein's personal notebook](https://github.com/stephane-klein/personnal-notebook) - for the style, not the content

## The Problem

- A Lot of contributors - and we want that number to go up, the higher the best. So we need to scale.
- The contributors don't know each others, come from different background, culture.
- The contributors have _different motives_
- The contributors have different skillsets
- The contributors have different time availabilities
- The contributors want to commit to the DAO at different levels (lightly as a hobby to 100% as a full-time job)
- The contributors have different work habits
- Some contributors are bad actors (bad actors are already plague in all organizations - but especially in the crypto space - see social engineering attack such as https://twitter.com/thomasg_eth/status/1492663192404779013?s=21). We want to isolate and throw away bad actors as fast as possible because they can and will _destroy_ any organization if left unaddressed.
- The contributors primarily don't trust each other (mainly because of the reason above)

In many ways, this is a _known problem, already addressed by open-source communities_, and discussed widely (see inspirations).

## The Solution

### Ideologically

- Like Hintjens suggests, to motivate people we need [Crazy, Beautiful and Easy](https://zguide.zeromq.org/docs/chapter6/#Crazy-Beautiful-and-Easy):

> You need a goal that’s crazy and simple enough to get people out of bed in the morning. Your community has to attract the very best people and that demands something special. With ZeroMQ, we said we were going to make “the Fastest. Messaging. Ever.”, which qualifies as a good motivator. If we’d said, we’re going to make “a smart transport layer that’ll connect your moving pieces cheaply and flexibly across your enterprise”, we’d have failed.
>
> Then your work must be beautiful, immediately useful, and attractive. Your contributors are users who want to explore just a little beyond where they are now. Make it simple, elegant, and brutally clean. The experience when people run or use your work should be an emotional one. They should feel something, and if you accurately solved even just one big problem that until then they didn’t quite realize they faced, you’ll have a small part of their soul.
>
> It must be easy to understand, use, and join. Too many projects have barriers to access: put yourself in the other person’s mind and see all the reasons they come to your site, thinking “Um, interesting project, but…” and then leave. You want them to stay and try it, just once. Use GitHub and put the issue tracker right there.
>
> If you do these things well, your community will be smart but more importantly, it will be intellectually and geographically diverse. This is really important. A group of like-minded experts cannot explore the problem landscape well. They tend to make big mistakes. Diversity beats education any time.

You Must have _clearly_ defined the goal and the values of your organization and then leave the rest to the community.

It's a democracy, it's decentralized BUT the project founders are VERY IMPORTANT. They set the goal for the organization, they are the _safeguards_ of the organization. Their role is to severely punish bad actors, and encourage good actors. Bad actors are bad because they don't abide to the explicit laws - a Protocol like [C4](https://hintjens.gitbooks.io/social-architecture/content/chapter4.html).

Little by little, good contributors can be promoted to `maintainers`. Maintainers are like project founders, they validate the work of good contributors and punish/expell bad actors.

Contributors should be put up to speed FAST.

The very first minutes a new contributors join in, he must have the tool to take action according to its specific skillset.

After contributing to something, the feedback (accepting his contribution) SHALL be almost immediate. This generates happiness in the contributor brain who immediately feels attachment, and hence will be happy to keep contributing. It means that it is important to accept a technically incomplete action - and modify/improve it later instead of making the contributor wait for months before his action/proposals advance or is accepted. After being accepted he/she will be happy to take feedback and improve.

The barrier of entry should be minimal which require VERY STRONG opsec, and especially in relation with software security (to which documents/information do the contributor has access to? how and who authorize him/her?). The contributor must not have to wait for others and ask for too many information.

Focus on the fewest communication platforms possible in order not to lose everybody because of too many tools.

Streamline work in order to have as much async written communication focusing on specific topics within the context of a precise processus, instead of large-scale live meetings going nowhere.

### In practice - tooling and processes

- Use Discourse ONLY except for sensitive private conversations. Why Discourse?

  - Discourse is self-hosted, no risk of being banned by Discord/Telegram whatsover
  - Discourse is very easy to use for non-technical people
  - Discourse can be _heavily_ and _easily_ customized (including visually) to suit the DAO specfic needs. Example: https://forum.hoprnet.org/
  - In particular, you can easily _vote_ on Discourse
  - Discourse can have a strong authorization mechanism, the same Discourse can not be the same for 2 users depending on their rights if necessary
  - Discourse is NOT a real-time chat so people actually _take time to think before writing_, and this way it is easier to prevent SPAM and NOISE

The DAO SHALL abide by the specific rules:

- Have a Sexy and Concise motto/goal BUT have a precise and comprehensive definition as to what is allowed, what is not, what is the precise goal of the organization, what are the values, and what happens if you trespass them. Write this down in a document following the protocol style. An example is [C4](https://hintjens.gitbooks.io/social-architecture/content/chapter4.html).
- Every conversation on Discourse SHALL be PUBLIC
- Basically 3 statuses: project founders, contributors and maintainers
- Project Founders are maintainers of all pods
- By default everyone is a contributor to every pod
- Good actors (contributors who have contributed quality work) SHOULD be proposed to become MAINTAINER role directly
- Use a password manager with ADVANCED authorization mechanism such as [1password Business](https://1password.com/teams/pricing). 1password Business also serve as a secure Cloud to share documents. Project Founders SHALL remain the sole OWNER/ADMIN of the password manager.
- Project founders SHALL REMAIN the sole Gnosis Safe Owners for security's sake
- Project founders MAY create smaller accounts/gnosis safe and give away control to them to trusted maintainers (good contributors who have proven themselves) to carry on operational tasks with a specific budget
- Project founders SHOULD create sub vaults within the password manager to share sensitive documents & credentials with specific pods
- Maintainers in pods SHOULD create as many subpods as possible with associated specific password manager's sub vaults
- No need to ask for permission if you're doing something that's not harming the DAO or doesn't cost money
- If the action requires money, then the contributors should draft a proposal
- Only the maintainers of the specific pod and the project owners vote for a proposal to be accepted for a Snapshot general vote
- Project Founder vote count for the same as a maintainer
- Project Founders SHALL veto if the proposal is against the core values of the DAO

### Incentives

- We all know that the success story of Bitcoin relies on its smart economical incentives
- However, economical incentive is NOT the most important here. Bitcoin's story is one person running his computer and receiving free money. The money incentive is baked into the protocol. Bitcoin miners don't need to talk to each other at all. They can be enemies, and it's actually a feature. The purpose is totally different than with a DAO which tries to find common grounds between people towards a specific goal. To function, a DAO needs human organizations, whereas Bitcoin network functions in a pure cold-blooded and neutral way (it's just infrastructure).
- The most important is recognition. A thank you. And the feeling of belonging. See [Dan Allen video](https://www.youtube.com/watch?v=a_vqg-go8XI)
- As an example, I have contributed to Gitcoin issue and received money, which is nice, but my code wasn't merged in production despite many thank you, and I didn't feel welcome to contribute more. On the other side, I have received a $10 T-Shirt for contributing to RedHat's codebase, and my code was immediately merged with a very smooth process experience. I felt better with the second option.
- Plus, in crypto, many people are here only for the speculative part of it. Those people can be considered either bad actors which will find any way to get money for free, or bad workers: who is interested in an employee whose only motivation is money?
- It's better to give people coins and block it for 10 years or until a milestone for the purpose of the DAO has been reached. It gives people a sense of alignment, a sense of belonging. Besides it is good for the asset's price because you can lock a large portion of the supply.

### Summary

#### Who can draft a proposal?

Everyone.

![draft_proposal](./draft_proposal.png)

#### Who can vote for a proposal to held a Snapshot vote?

Project Founders and maintainers:

![voting_proposal](./voting_proposal.png)

#### How is opsec organized so contributors are up to speed asap and everyone feels ownership?

![opsec](./opsec.png)

#### How are contributors paid? (if they want)

In a blocked account for 10 years+ or until an important milestone is achieved.

#### What are the KPIs?

TBD by the specific DAO. Can be the number of new contributors interacting in the Discourse. The number of maintainers being promoted. The number of people arriving divided by the number of people leaving. The number/evolution of number of active contributors? The action taken?

#### Who can ban/sanction a bad actor?

Both maintainers and project founders can ban bad actor. It should be done according to the protocol C4-like that had been drafted. Clear rules should be created with clear sanctions.

#### Who can revoke maintainers?

TBD in the organizational protocol. But probably maintainers and should be able to vote to revoke their peer maintainers or sub-maintainers (make them just contributors). Sub-Maintainers are maintainers of a sub-pod of the pod.

#### Who can veto a proposal?

Only Project Founders can veto proposal. But this could be adapted in the specific C4 protocol.

## License

BSD-2-Clause Plus Patent License
