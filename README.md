## Daniel Whitston

Zero-to-one architecture in fast-moving AI, building engineering organisations, and the assurance work that opens regulated markets.

[Highlights](#highlights) | [Experience](#experience) | [Technical grounding](#technical-grounding) | [Education](#education) | [Code](#code) | [Talks and media](#talks-and-media) | [Interests](#interests) | [Contact](#contact)

Founding CTO at [AutogenAI](https://autogenai.com/), employee #1 since the first commit in July 2022. I have owned the product architecture, the engineering organisation, the technical strategy and the company's regulatory position from an empty repository through seed, Series A and a $39.5m Series B, to a team of forty across the UK, US and Australia and FedRAMP High authorisation.

Before that, CTO at Policy in Practice, a Rails developer, a convention founder, and fifteen years in and around welfare-to-work, writing and winning the government-funded bids that AutogenAI's software now writes. London.

More on [whitston.uk](https://whitston.uk) and [LinkedIn](https://www.linkedin.com/in/danielwhitston).

## Highlights

* **Four generations of application architecture, one codebase, no rewrite event:** GPT-3 completions in 2022, then retrieval, then multi-model routing and evaluation, now agentic workflows with tools and skills, while the models underneath moved from GPT-3 to the current GPT, Claude and Gemini frontier.
* **Took AutogenAI into the US federal market** through Palantir FedStart, delivering FedRAMP High authorisation in January 2026, listed on the FedRAMP marketplace and now carrying authorisation letters from multiple federal agencies.
* **Zero to Series B.** Built AutogenAI's product from nothing, live with its first customer in autumn 2022 on GPT-3 completions, a few weeks before ChatGPT launched. Series A of $22.3m (Blossom Capital) and a $39.5m Series B co-led by Salesforce Ventures and Spark Capital in December 2023, both within eighteen months of the first commit; $65m raised in total across three rounds.
* **Built a 40-person global organisation** spanning engineering, ML, product, design, platform, IT and governance, risk and compliance, across three continents and time zones, then hired my own early responsibilities away to dedicated leaders as the company grew.
* **Privacy by design since 2023.** Research use of client data runs on tracked, organisation-level opt-in with role-gated access and hard blocks for organisations that declined, so "do you train on our data?" has had a one-line answer in every security questionnaire since.

## Experience

**Chief Technology Officer at AutogenAI (Jul 2022 - present)**    AutogenAI builds LLM software for writing bids and proposals. Its customers are organisations that win their work by bidding for it: aerospace and defence primes, outsourcers and government-services firms, the large consultancies, transport and infrastructure operators, and social-purpose providers running frontline services. They buy software the way regulated organisations do, so much of the job has been assurance.

*Product and architecture*

* Kept one architecture through four generations of LLM application design, from single-vendor GPT-3 completions to a routing and evaluation layer across GPT, Claude and Gemini and, in 2026, agentic workflows with visible task plans and streaming output.
* Joined as first employee with a founder, a thesis and no product, engineers or infrastructure. Hired the first NLP engineer within three weeks, made the early architectural calls (multi-tenant SaaS on AWS, and request-inspection tooling that let prompt engineers see exactly what was sent to and returned from the model, which grew into the AI quality workbench) and hired DevOps, backend and frontend around them.
* Led the 2026 move from long-running multi-step generation to agentic workflows with visible, editable task plans and streaming output, so users can see and steer what the system is doing while it runs. Ran a short improvement sprint on the existing generation path in parallel, and put prompt content on a refresh cycle with domain experts.
* Designed the 2023 mechanism for research use of client data, with a privacy-notice change, tracked opt-in by organisation, role-gated access and hard blocks for organisations that declined.
* Run a standing workstream consolidating four years of generation services onto a small number of shared paths to the model.
* Put LLM spend under joint management with finance: a standing platform-costs group, prompt caching (I instrumented the cache-usage tracing myself when the spans were missing), routing each task to the least expensive model that meets its evaluation bar, and caching in the retrieval layer.

*Team and organisation*

* Grew the function from myself to roughly forty people across engineering, ML, product, design, platform, IT and GRC in the UK, US and Australia. Ran product, design, research, GRC and IT directly until each had a leader, then handed them over in working order to a Head of Product who grew into CPO, a VP Engineering and a VP Platform, keeping architecture direction, federal strategy, the technical sales interface and security: acting CISO throughout, accountable for information and platform security over the Head of GRC, and named as system owner in the IRAP assessment.
* Built the engineering progression framework from scratch: six levels, five specialisms (technical team leadership, engineering management, architecture, thought leadership, AI engineering), progression profiles from junior to principal, job descriptions for every hiring role, and executive role definitions. Ran the annual review cycle against it, personally reviewing the leads.

*US federal market and compliance*

* Selected Palantir FedStart, sponsored the programme and owned the regulatory position while the VP Platform led delivery, and reached FedRAMP High in January 2026. Every customer migrated; federal release cadence now roughly matches commercial.
* Drove the GCC High SharePoint integration from "different Microsoft cloud, unclear API support" to live with a first client in June 2026.
* Completed and evidenced OWASP ASVS and SLSA supply-chain self-assessments as part of the FedRAMP audit programme.
* Own the regulatory portfolio: SOC 2 Type II, FedRAMP High, ISO 27001/27017/27018, Cyber Essentials Plus, Defence Cyber Certification Level 2, IRAP assessed at PROTECTED, TX-RAMP Level 2, Essential Eight alignment, CMMC 2 alignment, ITAR handling in the federal environment, and data-sovereignty positioning across three continents.
* When customers required a model vendor excluded, built it as a platform capability with an interim manual route, a standard letter and a compliance record, because the paperwork is what their auditors check.

*Commercial and customer-facing*

* External technical voice of the company: architecture and security reviews with enterprise buyers, technical due diligence, federal deal shaping, conference talks and customer briefings. Several of the largest logos arrived through diligence processes I fronted.
* Stood up a US engineering team from a standing start in two months in 2026: a forward-deployed engineering function, with the role defined and two FDEs hired including its lead; three UK engineers seconded to the US office on a week's notice; and the product researcher, all working directly with US staff and customers on US-specific functionality. Wired the team to sales through the fortnightly engineering and US sales cadence, so field intelligence changes engineering priorities within a fortnight.
* Ran presales technical assurance as a tracked queue covering vendor security questionnaires, AI-governance questionnaires, RFP security sections, DPAs and architecture reviews with customer security teams in the UK, US and Australia, answered from what we actually do, including talking prospects out of on-prem when the costing did not support it.

*Engineering operations and reliability*

* Gave reliability the go/no-go on the company's largest product release, a full redesign that reached GA in 2026 on the date committed in the launch plan, with a readiness decision that had an owner and a record, a launch checklist, and a structured post-launch review that reconciled telemetry with field reports.
* Drove a single severity and SLA system across engineering, support and product through a working group: shared definitions of support request, incident and near miss, an S1 to S5 ladder with response and mitigation SLAs, mappings into Linear and Datadog, and a capability-weighted availability model so service health reflects partial degradation.

*Recent code*

* My job is architecture and review. I keep enough recent code in the estate to stay credible in both: request success and failure logging across the main service (my PR, during the redesign reliability push), a geometric chunk-shrink fix for context-window overflow, tracing in the LLM service, and a solo procurement-system integration spike. None of it displaces team ownership.

*How I run things*

* **AI-written communication.** Rules set in 2026: if a model wrote it, you read it before you send it. Teams may set stricter rules, and machine-generated commentary goes where people can look it up and stays out of the channels they have to read.
* **Hiring mix.** Senior-heavy, with the reason written down. On a team using AI coding tools, the constraint on junior engineers is the quality of the tests and review around them. The decision has a written condition for revisiting it.
* **Engineering and US sales.** A fortnightly call with a fixed agenda and a written recap after each one, with owners and dates, which anyone can correct. It is where field intelligence changes engineering priorities and engineering changes reach the field.
* **Federal sales enablement.** Briefings on FedRAMP's move to Classes A to D, an answer to "we'd rather have Moderate", a one-page summary of what we hold, and a rule that IL5, IL6 and on-prem deployments are scoped jointly by sales and engineering before anything is committed to a customer.
* **Customer compliance claims.** When a customer cites a regulation we do not think applies, check the regulation, ship the fix anyway where it is cheap, and take the control interpretation from the authorising boundary.
* **Incidents.** Severity is set against the written definitions and corrected without pulling responders off the fix; every alert is acknowledged, with one named daily first responder rotating with the release rota; an incident closes once the service is confirmed healthy, which is later than the merge; and any failure that monitoring did not catch gets monitoring as part of the fix.

**Chief Technology Officer at Policy in Practice (Nov 2018 - Sep 2020)**    A govtech business selling welfare and benefits software, policy research and consultancy to local authorities, central government and the organisations delivering services for them. Built an in-house software function from the ground up to take over from a departing outsourced team with no break in service, while keeping SaaS platforms serving tens of thousands of users daily healthy and gradually replacing the legacy systems underneath them. Recruited my own successor before leaving for a sabbatical, and supported the transition as a consultant afterwards.

* Recruited and managed a team of 5 developers, and worked with them on code quality, peer support and self-management
* Planned, ran and evaluated development sprints; managed and delivered the technology roadmap
* Minimised, resolved and learned from service incidents; oversaw information security and data protection compliance
* Evaluated new systems and infrastructure and rearchitected for performance, resilience and flexibility
* Produced project specifications and costings, and advised the wider organisation on technology decisions
* Supported sales and operations staff with regular client contact, internal support and product usage analytics
* JavaScript, Node.js, TypeScript, Angular, MySQL, PostgreSQL, GitHub, AWS, CircleCI and Jira

**Developer at Homeflow (Jul 2017 - Nov 2018)**    Rails developer working on websites as a service for hundreds of estate agents and millions of weekly users, primarily on backend monoliths, with dozens of Linux servers and MySQL databases.

* Maintained large legacy code bases with millions of active users and hundreds of clients, and migrated them piecemeal to newer, more maintainable applications
* Created new functionality in discussion with clients and partners; implemented Rails major version upgrades
* Code review, sprint planning, retrospectives, improvements to CI processes
* Ruby, Rails 2/3/4/5, RSpec, MySQL, Jira, GitHub, BitBucket

**Freelance web and welfare consultant (Mar 2010 - Jun 2017)**    Web development, application design, product management, online community building and operations management for a range of clients. Notable assignments included:

* **Policy in Practice (Mar 2013 - Jan 2014, Nov 2015 - Mar 2016)**    Covering multiple areas at a high-growth startup combining SaaS tools with welfare research and consulting. Product managed the development of the Universal Benefit Calculator, across programming, operations and design functions in multiple countries
* **British Association for Supported Employment (2010 - 2016)**    Built and maintained the membership body's Drupal site, with delegated member management, a faceted knowledge base, targeted newsletters and a geolocated office search
* **Kennedy Scott (Sep 2014 - Feb 2015)**    Interim Business Development Director, leading business growth, new markets and bid team management for a medium-sized welfare-to-work and training organisation, and recruiting my permanent replacement
* **Benefits and Work (May 2012 - Apr 2013)**    Community management, customer support
* **Jobinasecond (Oct 2012 - Feb 2013)**    Service design, community management
* **Indus Delta (Mar 2010 - Apr 2011)**    Technical support and server management for the company I had founded and sold

**Founder of Nine Worlds (Sep 2012 - Aug 2018)**    Director of a multi-genre residential geek culture convention, taking place every August in London. Responsible for brand, web development, e-commerce and all information systems, ticketing, operational management, business planning and finance, marketing and comms, and a great deal of customer service. 1,500 attendees, with coverage in SFX, the Guardian, the Daily Mail and wider press.

**Trustee of the Policy in Practice Foundation (Apr 2014 - Apr 2018)**    Board member for a welfare research and policy charity.

**Founder of Indus Delta (Feb 2007 - Feb 2010)**    Built and sold the UK's most popular online welfare-to-work community and news source, with data tools and resources for employment-related providers and anyone interested in welfare reform and delivery. Read by almost all senior professionals in the sector. Sold as a profitable going concern to Inclusion (now the Learning and Work Institute) in 2010.

**Director of Special Projects at Kennedy Scott (Sep 2001 - Jan 2007)**    Created, marketed and managed government-funded programmes helping people into sustainable employment for a welfare-to-work provider. Bid for and won dozens of programmes, ranging in value from £5k to over £5m.

**Volunteer Development Worker at VSO Cameroon (Aug 1999 - Aug 2001)**    Taught Maths O Level, Physics O and A Level, and Computer Studies in a locally run school. Developed a careers advisory service with fellow teachers, organised and co-ran a weekend teacher training conference, and bid for and obtained funding to improve teaching facilities. Still the hardest job I have had.

**IT Manager at Yeoman Pressings (1998 - 1999)**    First job out of university, running IT for a manufacturing firm.

## Technical grounding

Accountable for AutogenAI's architecture and engineering from the first commit: a TypeScript-primary estate with Python services and a C# export service on .NET 9, deployed by Helm onto Kubernetes across roughly thirty environments on AWS, with a US federal environment operated within Palantir FedStart. Current judgement across LLM orchestration, retrieval, multi-model routing, evaluation and guardrails, observability (Datadog), and the compliance tooling that sits around all of it.

Earlier: Node.js, TypeScript and Angular at Policy in Practice, and Ruby on Rails at scale at Homeflow. Before that, programming informally since childhood (Spectrum BASIC and graph-paper sprites, then AMOS on the Amiga), through programming courses inside a maths degree, teaching programming and web design on a VSO placement, and a decade of building and hosting Joomla and Drupal sites for Kennedy Scott, Indus Delta, Nine Worlds and half a dozen others. Makers Academy in 2015; first professional developer role at Homeflow in 2017.

## Education

**Birkbeck, University of London (2020 - 2022)**    MSc Computer Science. Modules included Fundamentals of Computing, Computer Systems, Software Design and Programming, Information Systems, Data and Knowledge Management, and Cloud Computing.

Final project: *[A modelling engine for UK welfare benefit entitlement and household income](https://github.com/danwhitston/benefits-modeller)*. Existing benefit models are proprietary and cannot be audited or verified, and none of them integrate with automated theorem provers. I designed Ben, a domain-specific language for benefit rules, with a narrative language definition and a formal ANTLR4 grammar, a Python parser, and a runner that compiles Ben rules and test cases into the Z3 SMT solver. The proof of concept modelled Universal Credit eligibility and award rules and could solve for missing values in either direction, test hypotheses about rule changes as satisfiability problems, and emit proofs of assertions. The report covers the limits (scalability, usability, and that vertical slices beat horizontal layers) and what to do next.

**Makers Academy (2015)**    Sixteen-week intensive computer programming and web development bootcamp. Ruby, Rails, Sinatra, JavaScript, TDD, CI and agile practice.

**London Metropolitan University (2002 - 2004)**    PGDip Management Studies

**University of Warwick (1995 - 1998)**    BSc Mathematics

## Code

Most of my working code since 2018 has been in private company repositories. A few public things:

| Project | Description | Technologies |
|---|---|---|
| [whitston.uk](https://github.com/danwhitston/whitston.uk) | Personal site. A migration of a 2010 to 2017 Jekyll blog to Astro with every old URL redirected, a single-sourced profile config that drives the copy, metadata, JSON-LD and a build-time OG image, and a content check that rejects withdrawn phrasing and unfilled placeholders. | Astro, TypeScript, GitHub Actions to GitHub Pages, Cloudflare |
| [auction-api](https://github.com/danwhitston/auction-api) | MSc Cloud Computing coursework. A RESTful auction API with token auth, a cron-driven auction closer and a Python test client that exercises the public interface end to end. | Node.js, MongoDB, docker-compose, pytest, CI/CD to Google Cloud |
| [benefits-modeller](https://github.com/danwhitston/benefits-modeller) | The MSc final project described above: the Ben language, its ANTLR4 grammar, the parser and the Z3 runner, with the full project report in the repo. | Python, ANTLR4, Z3 |
| [cloud-computing-class](https://github.com/danwhitston/cloud-computing-class) | Lab exercises for the Birkbeck Cloud Computing module, worked on GCP and Azure. | Python, GCP, Azure |
| [contact-tracker](https://github.com/danwhitston/contact-tracker) and [rails-docker](https://github.com/danwhitston/rails-docker) | A personal CRM, and a barebones dockerised Rails development environment. | Ruby on Rails, Docker |
| [nineworlds](https://github.com/danwhitston/nineworlds) | Static archive of the Nine Worlds website, formerly a Drupal 7 site with Drupal Commerce ticketing and delegated publishing. | HTML |

## Talks and media

* **The Digital Lighthouse** (Softwire podcast, hosted by Zoe Cunningham), 15 May 2023: *How I've embraced AI and large language models*, 25 minutes on building an enterprise product on GPT-3 before ChatGPT. [Apple Podcasts](https://podcasts.apple.com/us/podcast/daniel-whitston-cto-how-ive-embraced-ai-and-large/id1457731478?i=1000696487278)
* **CTO Craft Bytes: Untangling GenAI**, at QuantumBlack's London offices, 19 September 2023: panellist on getting started with generative AI, its effect on the tool stack and its common pitfalls, alongside a QuantumBlack partner and the co-founder of an LLM inference startup, moderated by a fellow CTO. [Eventbrite](https://www.eventbrite.co.uk/e/cto-craft-bytes-untangling-genai-tickets-698407203747)
* **Canberra, February 2025**: panellist, "The Transformative Impact of AI on the Defence Industry", an AutogenAI round table for businesses supplying and consulting to the Australian defence industry, alongside a KPMG partner and the founder of BenchOn, moderated by a defence AI and robotics specialist. [LinkedIn](https://www.linkedin.com/posts/danielwhitston_autogenai-hosted-a-round-table-event-this-activity-7297155022167908353-jVDE)

## Interests

I read constantly, run regularly, and enjoy cooking. I'm interested in new technologies, social inclusion, and loud music.

## Contact

You can reach me on dan@whitston.uk.
