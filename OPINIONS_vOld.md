# OPINIONS

## Agentic Software

- Humans should review intent, constraints, and verification more than every line of agent-generated implementation.
  <!-- opinion-id: opinion-000001 -->
  <!-- sources: rw:01kkt3rryx42n2vw3vswnzn23c, rw:01kkt4ee5w23y80yqwmy77xpr0, rw:01kkvnzbr8p6g2vtr1wnxdf5g0 -->

- Making artifacts cheap to generate does not make ownership or comprehension cheap to skip: authors should verify, compress, and understand AI-generated work well enough to defend it, because handing an unedited output to multiple reviewers transfers the saved time downstream and can slow the organization.
  <!-- opinion-id: opinion-000002 -->
  <!-- sources: rw:01km6w5j2etpssfcbyjk75spx5, rw:01km6w6qb90sfan8c6dnfgrsx3, rw:01kt7p7hczwhjqkstr4zeqhpzx, rw:01kt7p7s76qx5c04gzkw0mn0tz, reader-summary:01kvehk4xt999exskypaf1a59y -->

- The human-owned artifacts in agentic software should increasingly be the product intent, acceptance criteria, architecture, program design, and verification contract. Architecture alone is not precise enough: before implementation, humans should review the shape of the code—including types, method signatures, program layout, and call stacks—so key design decisions are made explicitly rather than discovered during expensive code review.
  <!-- opinion-id: opinion-000003 -->
  <!-- sources: rw:01kkt4ee5w23y80yqwmy77xpr0, rw:01kkvnzbr8p6g2vtr1wnxdf5g0, rw:01kkt3pncjjjsrs8dv3pa3g4tk, rw:01kymktt0hjbm8sqa2aj3d7e3r -->

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

- Agent prompts and harnesses should simplify as models improve: give clear structure and canonical examples, but avoid sprawling if-else prompts that try to pre-solve every edge case. Treat every word and example as executable behavior—a single adjective can cause a quiet regression, and examples steer models more powerfully than written instructions—so prompt changes require evaluation rather than casual editing.
  <!-- opinion-id: opinion-000036 -->
  <!-- sources: rw:01kr1e39kwmpkhr3jmqz7ayjtz, rw:01kr1gd42xk8r6ttgm3as7dx56, rw:01kyg336anwz7nd06myrth3gys, rw:01kyg36dshvt3jzffb5193ew3p -->

- AI coding should be used as a learning loop, not just an issue-closing machine; if the model removes all friction without forcing hypotheses, explanations, and reflection, cognitive debt accumulates.
  <!-- opinion-id: opinion-000039 -->
  <!-- sources: rw:01ks4c170xt36eey5bq8sj0n5c, rw:01ks4c4wb18w1f86pc9dmj85ba, rw:01ks4c4zva18j35mcqvabwm870, rw:01ks4c5y6tq22mq95sm432mc83 -->

- Reliable agent harnesses should not treat bash or arbitrary code execution as universally necessary; many enterprise tasks are better served by task-specific, constrained tools. However, when a workflow must orchestrate many tool calls, letting the agent write and run a small program can be more efficient than selecting tools one turn at a time or calling them in a fixed order, because code can handle branching, parallelism, filtering, and retries deterministically. This expands the system’s attack surface, so execution should be sandboxed and permissions enforced below the model.
  <!-- opinion-id: opinion-000042 -->
  <!-- sources: rw:01kskq8p9jv6843n8xhktvc31b, reader-note:01kp70dfsh9taejhdym1d5qm4a, reader-note:01kqctk7cvpm01de2a4dbxn9hf, reader-summary:01ky84y2zeerdqhz9fdadmk0gy -->

- Agentic throughput is capped by human review bandwidth, not by how many workers the UI can spawn; the right amount of parallelism is the work you can actually evaluate without surrendering standards.
  <!-- opinion-id: opinion-000045 -->
  <!-- sources: rw:01kt868v6vctcfvazfy805hpmn, rw:01kt86bmyk96v9fbg4z9g1a945, reader-summary:01kvehk4xt999exskypaf1a59y -->

- A good vertical agent is a faithful compression of its task distribution: common capabilities belong in fast, always-loaded prompt context, rarer capabilities belong in discoverable tiers, and complete underlying references should remain searchable for the rare cases the curated layers do not cover.
  <!-- opinion-id: opinion-000047 -->
  <!-- sources: rw:01ktzkwnv9j8qwz0pe54r15dyr, rw:01ktzkxkv9845tfj42wc7qegbb, rw:01ktzm06bzb7fb6g4j2g639n96 -->

- Agentic optimization is only as good as its loss function: if the target, constraints, instruments, and examples leave cheap paths open, the agent will exploit them instead of getting genuinely better.
  <!-- opinion-id: opinion-000048 -->
  <!-- sources: rw:01kv16ca95y0hhdjhnxqf1zfzh, rw:01kv1x5hr6jvdszvnvn7zgx4p7 -->

- Building new software is learning under uncertainty; the right move is to expose the unknown parts to valuable feedback quickly, whether from CI, teammates, users, customers, or your own use.
  <!-- opinion-id: opinion-000049 -->
  <!-- sources: rw:01kts5rs2pw3jm9emexfz68dv8 -->

- Hand-tuned natural-language prompts become technical debt in production AI systems: each edge-case fix increases brittleness, slows iteration, and deepens model lock-in. Durable behavior should instead be defined by evals, metrics, and typed specifications, with prompts searched or generated against those measurements rather than treated as hand-crafted source code.
  <!-- opinion-id: opinion-000053 -->
  <!-- sources: reader-summary:01kw82hq01wyqj4pvtteyvwepy -->

- For long-lived code I care about, hands-off agent loops are not worth surrendering comprehension or design quality: present models compound local defensive fixes and fallbacks instead of enforcing strong invariants and making bad states impossible; they also duplicate code, invent weak abstractions, and cover unclear design with more machinery, leaving code more complex while only appearing more robust.
  <!-- opinion-id: opinion-000055 -->
  <!-- sources: rw:01kwakxpb46n3ypb93saym2cgt, rw:01kwam66dc9x2bx4wkk6samcj0 -->

- With coding agents by my side, I should treat almost any software problem as tractable. As investigation and fixes get cheaper, the differentiating skill is a “nose” for what isn't right—and the will to make it so.
  <!-- opinion-id: opinion-000064 -->
  <!-- sources: rw:01kxttky23nqp9erjgknbqgnkp, rw:01kxttm7devch5x32z8rv33mfd -->

- Coding-agent progress should be judged on long-horizon, evolving software work rather than short tasks whose only reward is passing tests. Short-horizon evals do not penalize eroding maintainability; benchmarks such as SlopCodeBench, which reveal requirements incrementally across successive issues, are a better signal—and currently show that models cannot be trusted to run real-shaped software work lights-off without steering.
  <!-- opinion-id: opinion-000066 -->
  <!-- sources: rw:01kyjz5qw5p4y9pp1pkdmqz9f1, rw:01kynf22gzg9grdfsxywjb9fv6 -->

- Long-horizon agents are a poor fit for truly novel product work because complete requirements do not exist upfront and present models cannot reliably judge what humans find intuitive, enjoyable, or valuable. They are better at reproducing known forms—like a Call of Duty clone whose requirements have already been absorbed into model weights—than inventing profitable new products alone; novel work needs tight human-agent loops that prototype, test with people, question the approach, and iteratively discover requirements.
  <!-- opinion-id: opinion-000071 -->
  <!-- sources: reader-summary:01kzme0d456m0s6yx9wrb0p2tk -->

- Agent performance depends on eliciting hidden constraints, not just receiving a task. Agents should ask one question at a time, prioritizing ambiguities whose answers could change the architecture; people should share their uncertainties and near-miss alternatives because why those options almost worked often reveals constraints—not merely preferences—more clearly than the final decision alone.
  <!-- opinion-id: opinion-000068 -->
  <!-- sources: rw:01kyr8198sjvr39g5y3wt1qeya, rw:01kyzqvd2bfzqqhz6bh9hjjdhv -->

## AI Leverage And Organizations

- AI rewards volition and domain expertise more than passive access: high-agency experts gain disproportionately because they choose worthwhile tasks, articulate what good looks like, challenge the model using a theory of the domain, and use the interaction to strengthen rather than atrophy their own capabilities. Terence Tao extracting a much deeper discussion of the recently discovered counterexample to the Jacobian Conjecture from the same ChatGPT available to everyone is the pattern in miniature. Education should therefore shift toward developing volition—the desire to work hard and put abundant knowledge to creative effect.
  <!-- opinion-id: opinion-000007 -->
  <!-- sources: rw:01knfbbfq8bs5rq4y3pry1qk8m, rw:01kkvb1sj4r2fnjczr3zdwyq9m, rw:01kncyags3eh05xj99e9b1kg19, rw:01kz46hcbds3p82ecg9f2s4z3c, rw:01kz4ak3s84yhqs7947rdcf481, rw:01kz7hfk8qpf650cnvq5af2jdp, rw:01kz7hgqd4ybpjefhecey60g91, rw:01kz7hgzsjq0qcyvfxxcf5wpfq, rw:01kz7hn26gzmf0c7z8zej6p21m -->

- Small AI-native teams can threaten larger organizations when they combine strong constraints, modular systems, fast feedback loops, and high-quality people whose shared trust and taste enable faster decisions. As AI makes execution cheaper, organizations should optimize for the new bottleneck—judgment—rather than reflexively adding headcount.
  <!-- opinion-id: opinion-000008 -->
  <!-- sources: reader-note:01kksyamfzmzcwz3z8hkxva94r, rw:01km1e1p2hm2qjwf64kyw2w8p7, rw:01kncyjj4a1pevhzz8qjetjsxv, rw:01kncykeak7bn6wawhf1ykqfar, rw:01kyr4wxpwcwxtm17xa9ns118t -->

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

- AI capability can improve quickly while economic takeoff remains slow, because a large share of GDP sits in inefficient government and government-subsidized sectors that will adopt AI—and use it effectively—only gradually.
  <!-- opinion-id: opinion-000070 -->
  <!-- sources: rw:01kz58hb1w75qrp3mq1e0y83ys -->

## Moats And Strategy

- Enterprise AI will optimize for intelligence per dollar: route bounded routine tasks to the cheapest model that reliably clears the quality bar, and reserve frontier intelligence for open-ended problems where extra capability creates uncapped value. As models commoditize, durable value may migrate toward orchestration platforms that make multi-model AI secure, reliable, compliant, cost-efficient, and integrated—not merely toward whoever owns the smartest model.
  <!-- opinion-id: opinion-000065 -->
  <!-- sources: reader-summary:01kwd7dyn5pxb7j2ydq53tcy24 -->

- Enterprise AI should minimize behavior change by embedding intelligence into existing workflows instead of requiring employees to open a new interface, remember when to use it, decide which tasks it applies to, and translate its output back into their real work.
  <!-- opinion-id: opinion-000067 -->
  <!-- sources: rw:01kyr5n200gq2ad40kx6wjfz4x -->

- Local and open-weight AI will not match frontier cloud models for the hardest work, but most everyday prompts are already close to a blind taste test, so cheaper models will handle the bulk of consumer queries and weaken cloud compute as a universal moat. Consumer AI pricing will approach zero and competition will shift toward privacy, features, interconnectivity, bundling, and the product or harness around the model, while frontier models retain a premium for coding, science, and other high-value work.
  <!-- opinion-id: opinion-000010 -->
  <!-- sources: rw:01kkt3a62sextfspc2qxdswkxf, rw:01kncy6rsmznccb4z4284w62yg, reader-summary:01kxer7f3s8sec8qvmdkpmw0zz -->

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

- As agent labor becomes cheap and commoditized, access to agents is not a durable moat. Companies should use that labor to accumulate what remains scarce—context, attention, trust, and brand—and turn those assets into differentiated outcomes through network effects.
  <!-- opinion-id: opinion-000069 -->
  <!-- sources: rw:01kz5858zt6m7msx2hj4f37k01 -->

- Expertise is dispersing from experts' heads into skills, SOPs, context files, and open-source projects, and once captured it never comes back out; advantages based only on undocumented expert memory will erode as AI reuses what gets captured.
  <!-- opinion-id: opinion-000021 -->
  <!-- sources: rw:01kp1x7w709ae4n44b0z3g7h4w -->

- In agent products, durable advantage should come from company-specific domain reasoning and business logic; the common stack underneath should increasingly be platform primitives rather than bespoke plumbing.
  <!-- opinion-id: opinion-000030 -->
  <!-- sources: rw:01kps6pym55wbe9p3jhk8mpd4x -->

- AI-native service firms and vertical application companies become defensible when delivery gets easier, faster, and better with each customer. Their durable asset is a tight learning loop that turns real customer workflows into vertical knowledge, reusable agents, process data, private benchmarks, and product features; a general lab is unlikely to run that loop as intensely because the vertical is not its main quest.
  <!-- opinion-id: opinion-000040 -->
  <!-- sources: rw:01ksk7bdz0gp2cdf3p1ctd280t, rw:01ksk7d2kahx9fp1brv5n7aqs1, rw:01ksk7dsefqbz5scnqznv9yyk9, rw:01kyr75e64axfk1p2h74gz78m9 -->

- Anything you can put on a leaderboard you can train against, so anything measurable is already on its way to commodity; durable value moves toward complex, private work that cannot be easily measured or copied.
  <!-- opinion-id: opinion-000050 -->
  <!-- sources: rw:01ktzm222bgxfw5cfbpdapyaet, rw:01kvpbkw1cdcwhbb15jakh3ae8, rw:01kvpbn4zp1z1vt0ea3rsh17ts -->

- Distribution-market fit comes before product-market fit: founders should know where customers spend time, whom they trust, and how they discover products, then build a distribution engine around those channels. A product cannot earn market love if the market never sees it.
  <!-- opinion-id: opinion-000051 -->
  <!-- sources: rw:01kvp4f50jt3eh3xmhgfr9sa3f -->

- A competitive model layer protects the application layer: customers want supplier diversity, labs want broad market share, and a better frontier model cannot cheaply reproduce an application's distribution, user habits, or deep workflow integration.
  <!-- opinion-id: opinion-000052 -->
  <!-- sources: rw:01kvpbszpjknaq87ptkvgzjzdp -->

- An agent product's interface should follow where its value and users live: build a dedicated core agent when users already live in your system of record or specialized domain reasoning justifies a vertical interface; when value lies in data or actions, power the horizontal agents where users already work through a headless API or MCP. Many products should do both, serving core users with an embedded agent and everyone else with the headless layer.
  <!-- opinion-id: opinion-000057 -->
  <!-- sources: reader-summary:01kwdzn0vfvbxpx25r0bwewy8c -->

- As software becomes easier to build, real, durable value requires extreme focus on truly ambitious problems rather than simple systems that anyone can create.
  <!-- opinion-id: opinion-000060 -->
  <!-- sources: rw:01kx8m8vnmn0ez2e8fb1xjwdj4 -->

- Early go-to-market should be run manually as a learning loop before it is automated: move through a testable thesis, prospecting, messaging, outreach, follow-ups, and a retro; maximize customer conversations; record the problem in customers' own words; and sharpen the ICP and positioning when repeated patterns emerge. Automate only after the message has proof, because premature scale hides the learning that makes the eventual sales machine work.
  <!-- opinion-id: opinion-000063 -->
  <!-- sources: reader-summary:01kxby2peknrqvm8v9j2qd3mmy -->

## Taste, Craft, And Signal

- Taste matters more when implementation gets cheaper, because AI makes features easy to add while excessive feature accumulation can reduce quality; the constraint shifts from "can this be built?" to "is this coherent, polished, and worth caring about?" Quality is often subtractive: simplicity requires understanding the product and user deeply enough to know what to remove, leave alone, or not build at all.
  <!-- opinion-id: opinion-000016 -->
  <!-- sources: rw:01kkt3bjqsny5edfmcbeertgxn, rw:01km6d48j613hq0c9n141x2d8s, rw:01km6d525k20c4d0wd7cnbys5e, rw:01knczdnkbndmvcm7v6qfcxyhp, reader-summary:01kw82jrbzr6qmpn06em2e28pw -->

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

- Taste is hard to create but valuable not because its outputs cannot be copied—they often can be copied almost immediately—but because it sets the standard others choose to copy: where objective metrics run out, consistently good qualitative judgment creates the reference point.
  <!-- opinion-id: opinion-000056 -->
  <!-- sources: rw:01kwawx9zm3s9wwzsh2htnkfme, rw:01kwawy67m3t1xcn3w939b28rr, rw:01kwawydzcs652tn0p9na08qbg -->

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

- As AI collapses the premium on routine implementation, software-engineering career leverage shifts toward mastering one hard production domain exceptionally well and developing real systems intuition about reliability, scale, security, performance, observability, and operational trade-offs.
  <!-- opinion-id: opinion-000054 -->
  <!-- sources: rw:01kwagqq4fmgg5ymmgwav25g79 -->

- In any fast-moving field, assume the latest information has not been written down yet; conversations with practitioners are therefore part of staying current, not merely networking.
  <!-- opinion-id: opinion-000058 -->
  <!-- sources: rw:01kwqmk418pzfvhs5wajx45n44 -->

- Early in a career, a high rejection rate can be evidence that you are aiming ambitiously enough. Deliberately applying beyond your expected reach builds the skill of absorbing “no” without surprise or dejection, so rejection stops narrowing the opportunities you pursue.
  <!-- opinion-id: opinion-000061 -->
  <!-- sources: rw:01kx9zx45d7vwgw0cc30m1hqz7 -->

- Luck is partly cultivated: because relevance is a weak proxy for whether a conversation will be useful, cast a wider social net and favor curious, enthusiastic people with broad interests. Repeated exploratory conversations can compound into the dense interpersonal networks that later look accidental.
  <!-- opinion-id: opinion-000062 -->
  <!-- sources: rw:01kx9zzyq4ye8m0psr5z7w0rjy, rw:01kxa0ejry5qqyyvvpjq0mn1sk -->

## Life And Community

- Meaning, aliveness, connection, and community are more likely to come from creating with other people than from consuming together or creating alone. Because shared creation requires initiation, planning, and social risk, it must be chosen deliberately rather than expected to happen by default.
  <!-- opinion-id: opinion-000059 -->
  <!-- sources: rw:01kx6fahxkrjq2yf7fj3jb5vkr, rw:01kx6favrrxs50y59g5cnhdy6k -->
