# OPINIONS

## Agentic Software

- Humans should review intent, constraints, and verification more than every line of agent-generated implementation.
  <!-- opinion-id: opinion-000001 -->
  <!-- sources: rw:01kkt3rryx42n2vw3vswnzn23c, rw:01kkt4ee5w23y80yqwmy77xpr0, rw:01kkvnzbr8p6g2vtr1wnxdf5g0 -->

- Making code cheap to generate does not make ownership or system comprehension cheap to skip; people should understand AI-generated artifacts well enough to defend them under questioning.
  <!-- opinion-id: opinion-000002 -->
  <!-- sources: rw:01km6w5j2etpssfcbyjk75spx5, rw:01km6w6qb90sfan8c6dnfgrsx3, rw:01kt7p7hczwhjqkstr4zeqhpzx, rw:01kt7p7s76qx5c04gzkw0mn0tz -->

- The human-owned artifact in agentic software should increasingly be the spec, acceptance criteria, and verification contract.
  <!-- opinion-id: opinion-000003 -->
  <!-- sources: rw:01kkt4ee5w23y80yqwmy77xpr0, rw:01kkvnzbr8p6g2vtr1wnxdf5g0, rw:01kkt3pncjjjsrs8dv3pa3g4tk -->

- AI makes implementation cheaper, but it does not make judgment cheap; the scarce work becomes deciding what is worth building, what good looks like, and whether an agent's output is actually good.
  <!-- opinion-id: opinion-000004 -->
  <!-- sources: rw:01kkvb1sj4r2fnjczr3zdwyq9m, rw:01knfbbfq8bs5rq4y3pry1qk8m, rw:01kncyags3eh05xj99e9b1kg19 -->

- Agents work best in constrained, legible, reversible environments where success can be checked and bad paths can be rolled back.
  <!-- opinion-id: opinion-000005 -->
  <!-- sources: rw:01km1e1p2hm2qjwf64kyw2w8p7, rw:01km1faax15sy6v2f8gcxrfaqv, rw:01kkt4hgxtq6yrb5yek8seytr6, rw:01kkt4hzc8s99v57absp2m39mg -->

- In AI-generated products, private eval sets, real user edge cases, specs, and verification artifacts are more durable than the artifact itself, because they encode what good means and what must remain true; SQLite's closed test suite is a clearer moat than its open source implementation.
  <!-- opinion-id: opinion-000006 -->
  <!-- sources: rw:01knfpajparaa0by09exzazyka, rw:01kkt3pncjjjsrs8dv3pa3g4tk, rw:01kkt4ee5w23y80yqwmy77xpr0, rw:01kv1xmg4addxx1z2p41kz4jbh -->

- As AI commoditizes scaffolding, the bottleneck moves to high-quality intent: having ideas worth pursuing, articulating what good looks like, and turning that intent into criteria that agents and organizations can optimize toward.
  <!-- opinion-id: opinion-000020 -->
  <!-- sources: rw:01kp1xajs4em2bhwcs3rz0j2wq, reader-summary:01kp1wzn737jegz28sg4ee3hzg -->

- Generalist base models are likely to beat domain-specific base models because intelligence from different fields builds on itself; domain-specific models mainly make sense if we hit physical limits in model size.
  <!-- opinion-id: opinion-000022 -->
  <!-- sources: reader-summary:01knheqfs4r61jy1ffvtbayqs8 -->

- Specs can shift implementation out of code, but they do not remove the need for precise design; a specification detailed enough to reliably generate working software starts to become code or code-like formal language.
  <!-- opinion-id: opinion-000025 -->
  <!-- sources: rw:01kp4spezcbaka7nxvzn7wm08h -->

- Agent systems should keep the harness thin, put reusable judgment and process in skills, and push repeatable execution into deterministic tools so model improvements compound without making reliability depend on the model.
  <!-- opinion-id: opinion-000026 -->
  <!-- sources: rw:01kp4ry1ctwkkkh49m80pbk6dm, rw:01kp4s1p54d7xewx3zfvv17wan, rw:01kp4s84v3vh8njpq3y815kcfn -->

- In agentic product work, Figma is in an awkward position: when the product ultimately lives in code, the design source of truth should move closer to executable code rather than a manual, pre-agentic replica of the system.
  <!-- opinion-id: opinion-000029 -->
  <!-- sources: rw:01kpph104zd1vdw0vkdqpsc6m9 -->

- Agent prompts and harnesses should simplify as models improve: give clear structure and canonical examples, but avoid sprawling if-else prompts that try to pre-solve every edge case.
  <!-- opinion-id: opinion-000036 -->
  <!-- sources: rw:01kr1e39kwmpkhr3jmqz7ayjtz, rw:01kr1gd42xk8r6ttgm3as7dx56 -->

- AI coding should be used as a learning loop, not just an issue-closing machine; if the model removes all friction without forcing hypotheses, explanations, and reflection, cognitive debt accumulates.
  <!-- opinion-id: opinion-000039 -->
  <!-- sources: rw:01ks4c170xt36eey5bq8sj0n5c, rw:01ks4c4wb18w1f86pc9dmj85ba, rw:01ks4c4zva18j35mcqvabwm870, rw:01ks4c5y6tq22mq95sm432mc83 -->

- Reliable agent harnesses should not treat bash or arbitrary code execution as universally necessary; many enterprise tasks are better served by task-specific, constrained tools than by a model with general computer access.
  <!-- opinion-id: opinion-000042 -->
  <!-- sources: rw:01kskq8p9jv6843n8xhktvc31b, reader-note:01kp70dfsh9taejhdym1d5qm4a, reader-note:01kqctk7cvpm01de2a4dbxn9hf -->

- Agentic throughput is capped by human review bandwidth, not by how many workers the UI can spawn; the right amount of parallelism is the work you can actually evaluate without surrendering standards.
  <!-- opinion-id: opinion-000045 -->
  <!-- sources: rw:01kt868v6vctcfvazfy805hpmn, rw:01kt86bmyk96v9fbg4z9g1a945 -->

- A good vertical agent is a faithful compression of its task distribution: common capabilities belong in fast, always-loaded prompt context, rarer capabilities belong in discoverable tiers, and complete underlying references should remain searchable for the rare cases the curated layers do not cover.
  <!-- opinion-id: opinion-000047 -->
  <!-- sources: rw:01ktzkwnv9j8qwz0pe54r15dyr, rw:01ktzkxkv9845tfj42wc7qegbb, rw:01ktzm06bzb7fb6g4j2g639n96 -->

- Agentic optimization is only as good as its loss function: if the target, constraints, instruments, and examples leave cheap paths open, the agent will exploit them instead of getting genuinely better.
  <!-- opinion-id: opinion-000048 -->
  <!-- sources: rw:01kv16ca95y0hhdjhnxqf1zfzh, rw:01kv1x5hr6jvdszvnvn7zgx4p7 -->

- Building new software is learning under uncertainty; the right move is to expose the unknown parts to valuable feedback quickly, whether from CI, teammates, users, customers, or your own use.
  <!-- opinion-id: opinion-000049 -->
  <!-- sources: rw:01kts5rs2pw3jm9emexfz68dv8 -->

## AI Leverage And Organizations

- Top builders and high-agency operators gain disproportionately more from AI than median users because they are better at choosing tasks, directing agents, and judging results.
  <!-- opinion-id: opinion-000007 -->
  <!-- sources: rw:01knfbbfq8bs5rq4y3pry1qk8m, rw:01kkvb1sj4r2fnjczr3zdwyq9m, rw:01kncyags3eh05xj99e9b1kg19 -->

- Small AI-native teams can threaten larger organizations when they have stronger constraints, modular systems, and faster feedback loops.
  <!-- opinion-id: opinion-000008 -->
  <!-- sources: reader-note:01kksyamfzmzcwz3z8hkxva94r, rw:01km1e1p2hm2qjwf64kyw2w8p7, rw:01kncyjj4a1pevhzz8qjetjsxv, rw:01kncykeak7bn6wawhf1ykqfar -->

- Many companies are sized for a world where scaling required more people, and agents may move the efficient size downward.
  <!-- opinion-id: opinion-000009 -->
  <!-- sources: rw:01kncyjj4a1pevhzz8qjetjsxv, rw:01kncykeak7bn6wawhf1ykqfar, rw:01kkt3c037a7gghx7jfxk0bbv2 -->

- AI does not need to beat an idealized version of knowledge work; in many companies it only has to beat messy, inconsistent operations where simply following instructions reliably is already above the current bar.
  <!-- opinion-id: opinion-000027 -->
  <!-- sources: rw:01kp4wgb37kpzj9jyq45a5nyk6 -->

- AI service replacement is most likely where customers already outsource repeatable execution or playbook-based work and judge the vendor by outcomes rather than visible effort.
  <!-- opinion-id: opinion-000037 -->
  <!-- sources: rw:01ks48kzxb83phc9391h8cf8rb, rw:01ks48m61rmne707ncmvybtzep, rw:01ks48n8bwnm9z99f78pykbdz0, rw:01ks48npm5g6axxxm14749q10z -->

- Enterprise AI transformation should start by mapping end-to-end workflows, ROI, data layers, and tribal knowledge around existing systems; rip-and-replace migrations often slow adoption more than they help.
  <!-- opinion-id: opinion-000041 -->
  <!-- sources: rw:01kskr0rbgy1rkw3y1gq9jw55g, rw:01kskr18czcpb0gsrgex1jn5qc, rw:01kskr1kaf1k792d3t6q8xj596 -->

## Moats And Strategy

- Local AI will not match frontier cloud AI for the hardest work, but it can still handle enough tasks to weaken cloud compute as a universal moat.
  <!-- opinion-id: opinion-000010 -->
  <!-- sources: rw:01kkt3a62sextfspc2qxdswkxf, rw:01kncy6rsmznccb4z4284w62yg -->

- Agent products are differentiated by model-plus-harness integration, not model quality alone.
  <!-- opinion-id: opinion-000011 -->
  <!-- sources: rw:01kncyqbhj7d8t10emepgzgt1s, rw:01knfkcj69ejbkezfnwj40j7qm, rw:01kkt4hzc8s99v57absp2m39mg -->

- AI commoditizes work that can be specified and verified, and increases the relative value of knowledge that can only be learned by operating in the real world.
  <!-- opinion-id: opinion-000012 -->
  <!-- sources: rw:01knfjsc5qjmyf0jd2k8yedkwm, rw:01knfjyjpmmeh1wpv1a4z2dy88, rw:01knfk2f4x3c2ne8vn10x52rgp -->

- Operational scar tissue compounds in coupled, shifting systems: if each real-world surprise changes how future surprises should be interpreted, a newcomer cannot catch up merely by studying the current state.
  <!-- opinion-id: opinion-000013 -->
  <!-- sources: rw:01knfjyjpmmeh1wpv1a4z2dy88, rw:01knfk2f4x3c2ne8vn10x52rgp, rw:01knfk4zd7ca5tq7kf760jht7a, reader-note:01kksy9drnnqysr6tb5e2n0pw3 -->

- A prototype can copy features, but it cannot copy the operational trust earned through reliability, audits, rollback discipline, and incident response.
  <!-- opinion-id: opinion-000014 -->
  <!-- sources: rw:01knfqmzt8f383ajbrs048naza, rw:01knfjsc5qjmyf0jd2k8yedkwm, rw:01knfk2f4x3c2ne8vn10x52rgp -->

- Brand becomes more important when substantive product differences become easier to copy.
  <!-- opinion-id: opinion-000015 -->
  <!-- sources: rw:01km6wb6fs62k46c08ymnb0aye, rw:01knfqmzt8f383ajbrs048naza -->

- Expertise is dispersing from experts' heads into skills, SOPs, context files, and open-source projects, and once captured it never comes back out; advantages based only on undocumented expert memory will erode as AI reuses what gets captured.
  <!-- opinion-id: opinion-000021 -->
  <!-- sources: rw:01kp1x7w709ae4n44b0z3g7h4w -->

- In agent products, durable advantage should come from company-specific domain reasoning and business logic; the common stack underneath should increasingly be platform primitives rather than bespoke plumbing.
  <!-- opinion-id: opinion-000030 -->
  <!-- sources: rw:01kps6pym55wbe9p3jhk8mpd4x -->

- AI-native service firms only become software-like when delivery gets easier, faster, and better with each client; the durable asset is vertical workflow knowledge, reusable agents, process data, and proof that the system compounds.
  <!-- opinion-id: opinion-000040 -->
  <!-- sources: rw:01ksk7bdz0gp2cdf3p1ctd280t, rw:01ksk7d2kahx9fp1brv5n7aqs1, rw:01ksk7dsefqbz5scnqznv9yyk9 -->

- Anything you can put on a leaderboard you can train against, so anything measurable is already on its way to commodity; durable value moves toward complex, private work that cannot be easily measured or copied.
  <!-- opinion-id: opinion-000050 -->
  <!-- sources: rw:01ktzm222bgxfw5cfbpdapyaet -->

## Taste, Craft, And Signal

- Taste matters more when implementation gets cheaper, because the constraint shifts from "can this be built?" to "is this coherent, polished, and worth caring about?"
  <!-- opinion-id: opinion-000016 -->
  <!-- sources: rw:01kkt3bjqsny5edfmcbeertgxn, rw:01km6d48j613hq0c9n141x2d8s, rw:01km6d525k20c4d0wd7cnbys5e, rw:01knczdnkbndmvcm7v6qfcxyhp -->

- Cheap "pretty good" AI output can crowd out deeper work by flooding the channel with plausible substitutes before anyone pays the cost to make the stronger version.
  <!-- opinion-id: opinion-000017 -->
  <!-- sources: rw:01km1mjh61x3a121avgb35ybmf, rw:01km6c0q40mev12z6d96mr7wtc, reader-note:01kkwkjsegskdveypma6jtppxa -->

- When AI makes output costless, volume stops being a reliable signal of effort, care, or productivity; AI-generated cover letters are an example because customization stops proving real interest.
  <!-- opinion-id: opinion-000018 -->
  <!-- sources: rw:01km1mjh61x3a121avgb35ybmf, rw:01km6c0q40mev12z6d96mr7wtc, reader-note:01kkwkjsegskdveypma6jtppxa -->

- The current AI slop era may be a golden age for human-AI work: models create useful slop at volume, humans are still needed to desloppify it, and that combination gives real leverage while keeping the work fun; if AI eventually displaces people or takes over the more interesting work, this moment may fade.
  <!-- opinion-id: opinion-000032 -->
  <!-- sources: rw:01kps7gne0fanp8tbn80gk6m75 -->

- In AI-assisted creative work, taste is not just knowing what you want but knowing what to reject: the default output is almost always generic, so have an opinion about the defaults — starting with the hook — and be willing to override them.
  <!-- opinion-id: opinion-000033 -->
  <!-- sources: rw:01kqx6150aqwx36jrn6m7w15mw, rw:01kqx62f1hr4jw9seen2t9k8xv -->

- When AI can cheaply generate repos, tests, and docs, real use becomes a stronger trust signal than polished artifacts; for serious software, prefer products with operational proof from yourself or comparable customers.
  <!-- opinion-id: opinion-000034 -->
  <!-- sources: rw:01kqza7w92hqnr2n1hratd69ja, rw:01kqzacv41vz7vwqtds7faevws -->

- Use agents to remove routine work that does not benefit from synchronous involvement, but stay deliberately in the loop where taste develops and original work needs you shaping it rather than just approving it.
  <!-- opinion-id: opinion-000046 -->
  <!-- sources: rw:01ktd4kw43j7714py2smmacmpt -->

## Career And Work

- A corporate job does not need to be personally meaningful if it is useful: building skills, funding independent projects, or buying time for higher-conviction work.
  <!-- opinion-id: opinion-000019 -->
  <!-- sources: rw:01knfjhr4hnp2exvcgpggvywsd -->

- Career growth is not something to wait for: managers can help, but ambitious people need to proactively tell their manager what they want, ask what must be true to reach the next level, and seek scope instead of assuming good work will be noticed.
  <!-- opinion-id: opinion-000023 -->
  <!-- sources: rw:01kp1xj8s4sdw2nswebpn7pher -->

- In hiring, an impressive accomplishment only creates signal if the candidate can deliver it well; a truthful, practiced account of tradeoffs and close calls reveals more than a polished success story that hides how they actually think.
  <!-- opinion-id: opinion-000024 -->
  <!-- sources: rw:01kp1wkxxh3a81jf620rm5kzns, rw:01kp1wnk6d4ckysfzsj34sfpfk, rw:01kp1wrn0b3b2ray7wa6yhf08e -->

- People do not need work specifically; they need four things work happens to provide — agency, contribution, mastery, and connection — so if AI displaces work, whatever comes after has to supply those four functions, not just income.
  <!-- opinion-id: opinion-000028 -->
  <!-- sources: rw:01kp4ymck943np90xtvj52v2fh -->

- Engineering interviews in an AI-native world should test how candidates scope, build, review, and reason with AI tools on representative product work instead of testing code mechanics without assistance.
  <!-- opinion-id: opinion-000031 -->
  <!-- sources: reader-summary:01kpxgvdm8h04w0k41wv4nrjgb -->

- Passive productivity like reading and podcasts is helpful, but it has diminishing returns; active productivity scales better because its returns compound the more time you spend creating.
  <!-- opinion-id: opinion-000035 -->
  <!-- sources: rw:01kr1c8j4a6aph5qyrbswghyyg -->

- Career leverage is not about being well-rounded; Price's Law suggests that a small square-root-sized minority produces much of the output, so the goal is to find and compound your √n multiplier skills into a rare combination.
  <!-- opinion-id: opinion-000038 -->
  <!-- sources: rw:01ks4a57xnehk7pvt344an40r0, rw:01ks4a6rrzwhhxew6vxs7d1h4k -->

- Career choices should be judged by the compounding assets they build - skills, reputation, network, options, and operational scars - not just immediate pay, title, or brand.
  <!-- opinion-id: opinion-000043 -->
  <!-- sources: rw:01ksv22qgqjrmckm733rhy3br4, rw:01ksv259vfm1xwns6ksyfcb3z0, rw:01ksvjrngk7z25y7ygtv1cd6rv -->

- High agency needs recovery and self-context, not endless escalation; because there is no final level, ambitious people should deliberately look back, accept their current state, and take breaks.
  <!-- opinion-id: opinion-000044 -->
  <!-- sources: rw:01ksjznkpkmd1p430mjrnt1dfa, rw:01kskp6r68fqp6eewx9v87pt8f, rw:01kskp7frjqgykp69s4ja2g51q -->
