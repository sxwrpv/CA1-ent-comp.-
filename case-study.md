The Transistor and Its Impact on Computing
1. Introduction
A computer is ultimately just a collection of microscopic switches. Whether it is a room-sized 1940s machine or a 2026 AI superchip, the core logic remains exactly the same: manipulating binary states (1s and 0s). The first electronic computers used vacuum tubes, heated glass bulbs that were big, hot and unreliable. ENIAC, completed in 1945, contained about 17,500 of them and filled a large room and was the world's first general-purpose electronic digital computer (CSMonitor, 1996).
In December 1947, researchers at Bell Telephone Laboratories demonstrated a different kind of switch, a small piece of semiconductor that could amplify and switch signals using far less space, heat and power. That was the transistor. Almost eighty years later, a single AI accelerator package holds hundreds of billions of them across several dies*.

The thesis is that the 1947 invention is only half of the explanation. The transistor reshaped computing because two things kept pushing each other forward, it was the symbiotic feedback loop between technological scaling and market economics that actually drove the digital revolution. Engineers found ways to build transistors in huge numbers and keep shrinking them: silicon, the planar process, the MOSFET** and CMOS***. Alongside that, patent licensing, spin-off companies and later specialised foundries turned the shrinking into an economic engine.

The evidence comes from industry histories (Riordan and Hoddeson, 1997; Lécuyer, 2006; Miller, 2022), technical papers, an economics study of the 1956 antitrust settlement and recent reports. Figures for modern chips come from company announcements and trade press

2. Historical Development

2.1 Before the transistor
A machine with thousands of tubes drew a lot of power, needed cooling and failed often enough to limit how long a calculation could run. Telephone networks had the same problem, which pushed Bell Laboratories, the research arm of AT&T, to build a solid-state physics group in the 1940s.

2.2 Invention, 1947 to 1951
In December 1947, John Bardeen and Walter Brattain, working in a group led by William Shockley, demonstrated the first point-contact transistor, made from germanium. Bell Labs announced it in 1948, and a colleague, John R. Pierce, suggested the name "transistor". Shockley developed the theory of a more durable design, the junction transistor, in 1948. Working junction devices followed in 1951 (Riordan and Hoddeson, 1997). All three men shared the 1956 Nobel Prize in Physics

2.3 From germanium to silicon, 1950s
Germanium transistors behaved badly at higher temperatures. On 14 April 1954, Gordon Teal at Texas Instruments (TI) showed a working silicon transistor, and he announced it publicly in May 10, 1954. Silicon tolerated heat better, though consumer products came first from germanium. The Regency TR-1 portable radio (The the world’s first commercially manufactured transistor radio), announced in October 1954 with TI transistors, was among the first mass-market transistor products

2.4 The integrated circuit and the planar process, 1958 to 1959
Even with transistors, building a computer meant wiring thousands of separate parts together by hand. People called this bottleneck the "tyranny of numbers". In September 1958, Jack Kilby at TI showed a circuit with several components formed on a single piece of germanium. In July 1959, Robert Noyce and Fairchild Semiconductor filed their own patent, which used Jean Hoerni's planar process to build transistors on a silicon wafer under a protective layer of silicon dioxide. Kilby later shared the 2000 Nobel Prize in Physics for the integrated circuit (IC).

2.5 The MOSFET and CMOS, 1959 to 1963
Mohamed Atalla and Dawon Kahng at Bell Labs invented the metal-oxide-semiconductor field-effect transistor (MOSFET) in 1959 and demonstrated working devices in 1960. It was easier to manufacture and to shrink than earlier designs. In 1963, Frank Wanlass and Chih-Tang Sah at Fairchild described complementary MOS (CMOS) logic, which pairs two types of transistor so that a circuit uses real power only when it switches. CMOS became the dominant architecture for digital microchips.

2.6 Moore's Law and the microprocessor, 1965 to 1971
In 1965, Gordon Moore noticed that the number of components on an integrated circuit had been doubling about every year, and he predicted that this would continue. In 1975 he revised the pace to a doubling roughly every two years, Moore co-founded Intel in 1968. In 1971 the company released the 4004, the first commercial microprocessor, with about 2,300 transistors and a 10-micrometre process.

2.7 Scaling to the present
For the next three decades, chipmakers shrank transistors on a steady schedule and got better speed, cost and energy use at once. That ran out around the mid-2000s, when leakage and heat stopped clock speeds from rising further, forcing an industry shift toward multi-core processors. The FinFET (Fin field-effect transistor), first described in the research literature around 2000, reached volume production in Intel's 22 nm chips in 2012 after being announced in 2011. Gate-all-around designs are now in production. TSMC (Taiwan Semiconductor Manufacturing Company) began volume production of its 2 nm node, its first gate-all-around nanosheet process, around the end of 2025. Chips have grown too, NVIDIA's H100 had about 80 billion transistors (2022), the B200 about 208 billion across two dies (2024), and the Rubin GPU announced in 2026 is reported to have about 336 billion

3.  Engineering Viewpoint
Developing the transistor required a small, reliable switch that used little power and was cheap to manufacture in large numbers. Silicon replaced germanium because it tolerated higher temperatures and formed a stable, insulating oxide layer. This oxide protects sensitive junctions and separates a MOSFET’s gate from the semiconductor, allowing its electric field to control current flow (Riordan and Hoddeson, 1997). Jean Hoerni’s planar process enabled batch fabrication, while photolithography transferred patterns onto wafers so devices could undergo the same steps. Advances allowed millions of transistors to be manufactured together. Costs depended on chip area, process complexity and the proportion of working chips, rather than transistor count alone. Smaller transistors meant more devices in the same area and a lower cost per transistor.

3.1 Integration and the “tyranny of numbers”
As circuits grew, wiring separate components became difficult and unreliable. Every connection introduced a possible failure. Kilby’s first integrated circuit still used wires, whereas the planar approach formed components and interconnections on the same chip (Lécuyer, 2006). Less manual assembly reduced wiring errors, and shorter connections improved speed.

3.2 MOSFET and CMOS: designing for power
CMOS reduced power consumption through complementary transistors that switch in opposite states. A settled gate ideally has no conducting path directly from supply to ground. Most power is consumed during switching, although devices also leak current. Low static power consumption allowed more logic within thermal limits, helping CMOS dominate digital circuits.

3.3 Scaling laws
Moore’s Law described transistor counts roughly doubling at regular intervals. Dennard scaling explained how smaller transistors could operate faster without increasing power density, provided their dimensions and operating voltage decreased together (Dennard et al., 1974). For decades, these trends supported higher performance and lower costs per transistor without a corresponding increase in power density.

3.4 Limits and adaptations
As gate insulators became only a few atoms thick, leakage increased, while further voltage reductions threatened reliable switching. Dennard scaling broke down around 2005–2007 (Esmaeilzadeh et al., 2011). Chips could contain more transistors, but power limits prevented all from operating at full speed simultaneously. Esmaeilzadeh et al. projected that roughly a fifth of a chip at 22 nm, and over half at 8 nm, might remain powered off as “dark silicon.”
Designers shifted towards multiple cores and specialised processors, including GPUs and AI accelerators. Transistor geometry changed: FinFETs place the gate around a raised silicon fin for better channel control (Hisamoto et al., 2000). Gate-all-around designs extend this approach.

3.5 Engineering evaluation
Progress depended on improvements in materials, device design and manufacturing, often at increasing cost. Fabrication demands expensive equipment and tighter process control. Smaller transistors still offer benefits, but no longer deliver the predictable speed and power improvements associated with Dennard scaling.

3.6 Engineering outlook
Scaling is expected to continue at greater cost. TSMC’s A16 process, featuring backside power delivery, reportedly shifted from late 2026 to 2027; A14 is targeted for 2028. Imec places CFETs at the A7 generation and two-dimensional channel materials later, with contacts, doping and integration still unresolved.
As chips approach the reticle limit, chiplets, high-bandwidth memory and advanced packaging offer further gains. Capacity remains a constraint for technologies such as TSMC’s 5.5-reticle CoWoS. TSMC’s COUPE brings optical connections into packages.
Neuromorphic photonic systems still require electronic control and conversion; their energy advantages over GPUs lack comparable benchmarking, IBM’s and Google’s quantum milestones around 2030 remain company targets.

4. Business Viewpoint
Licensing and the spread of the technology
The business story starts with an unusual decision. Bell Labs belonged to AT&T, a regulated monopoly. From late 1951, Bell offered transistor licences for $25,000 each and invited licensees to a symposium to learn the technology (PBS, n.d.-a). In 1956, AT&T settled a US antitrust case with a consent decree that made its existing patents available royalty-free and required future patents to be licensed at reasonable royalties. About 7,800 patents were affected, most of them from Bell Labs. Watzinger et al. argue that opening up the patents encouraged follow-on innovation. This causal claim is an interpretation, 
since military demand was also at work.

4.1 Silicon Valley and the spin-off model
William Shockley left Bell Labs to found Shockley Semiconductor Laboratory in Mountain View, California, in 1956. His management style was unpopular, and in 1957 eight of his engineers, later nicknamed the "traitorous eight", left. With funding from Sherman Fairchild's Fairchild Camera and Instrument, they formed Fairchild Semiconductor in September 1957. Fairchild became the training ground of the industry. Noyce and Moore left in 1968 to found Intel, and many other founders and executives followed in a chain of spin-offs. Knowledge travelled with people, and venture-style funding backed them.

4.2 Moore's Law as business strategy
Moore's Law is often described as a law of nature, but business analysts treat it more like a coordination device. Every generation was expected to double density at a lower cost per transistor, so companies planned products, factories and research budgets around that rhythm. Firms that fell behind were soon priced out, which made the law partly self-fulfilling. Early military and space buyers helped firms move down the learning curve, lower costs widened demand, and demand paid for the next generation of manufacturing.

4.3 Capital intensity and the foundry model
The same forces that made progress fast also made it expensive. Leading-edge fabs now run to many billions of dollars, and only a handful of companies can afford them. In 1987 Morris Chang founded TSMC as the first dedicated foundry, a company that makes chips for other firms and does not design its own (Miller, 2022). The industry split into "fabless" design firms, such as NVIDIA, AMD and Qualcomm, and the manufacturers. The model lowered the barrier for designers and set off a wave of innovation, but it also concentrated manufacturing in very few hands.

4.4 Value capture and concentration
Today the leading-edge supply chain runs through a few chokepoints. ASML in the Netherlands is the only commercial supplier of extreme ultraviolet lithography machines and expected to ship about 60 of them in 2026 (RTÉ, 2026). TSMC in Taiwan took about 72.5% of global foundry revenue in the second quarter of 2026 (TrendForce, 2026a), and Miller (2022) describes it as making most of the world's most advanced logic chips. AlixPartners (2021) forecast that the 2021 chip shortage would cost the car industry about US$210 billion in revenue and 7.7 million vehicles of production. It is a forecast, and chips were only one of several disruptions, but it shows how a hidden dependency can suddenly stop whole industries.

4.5 Business evaluation
From a business angle, the transistor is an enabling technology whose importance was shaped by market structure: permissive licensing and mobile talent produced extraordinary growth, and the same dynamics later produced concentration and a fragile supply chain.

4.6 Business outlook
The forecasts depend heavily on AI demand. WSTS (2026) raised its 2026 forecast from US$975 billion in December 2025 to about US$1.51 trillion, with memory up roughly 250% (BigGo Finance, 2026), and expects US$1.9 trillion in 2027. Part of this reflects price rises as much as extra units. Gartner forecasts DRAM prices up 125% and NAND up 234% in 2026 and puts 2026 revenue lower, above US$1.3 trillion (Intelligent CIO, 2026). The IEA (2026) expects data-centre electricity use to roughly double by 2030, and capital-heavy firms carry the most risk if demand slows. Intel, for example, plans 14A volume production in 2028 (Tom's Hardware, 2026) but is reported to tie the capital for it to external customer commitments (Tech Times, 2026).
7. Ethical Reflection and Improvements
Conclusion: 



References
AlixPartners (2021) 'Shortages related to semiconductors to cost the auto industry $210 billion in revenues this year, says new AlixPartners forecast', AlixPartners, 23 September.
Alberico, I. (2026) 'The Right to Repair Directive: what changes on 31 July?', Right to Repair Europe, 30 July.
Alvarez, E., Mehta, V. and Ghodsian, F. (2026) 'Inside NVIDIA Rubin GPU architecture: powering the era of agentic AI', NVIDIA Technical Blog, 21 July.
AndesQubit Research (2026) 'Quantum computing roadmap 2026 to 2030: IBM, Google, rivals', Andes Qubit, 23 September.
ASML (2026) ASML reports Q2 2026 financial results, 15 July.
Baldé, C.P. et al. (2024) The global e-waste monitor 2024. Geneva and Bonn: International Telecommunication Union and United Nations Institute for Training and Research.
Bile, A. (2026) 'Recent advances in neuromorphic photonics: devices, architectures, and physical learning systems (2022–2026)', Applied Physics Reviews, 13(3), 031339.
Cass, S. (2018) 'Chip Hall of Fame: Intel 4004 microprocessor', IEEE Spectrum, 2 July.
CHIPS and Science Act 2022, Pub. L. No. 117-167, 136 Stat. 1366.
Computer History Museum (n.d.a) '1947: Invention of the point-contact transistor', The Silicon Engine.
Computer History Museum (n.d.b) '1951: First grown-junction transistors fabricated', The Silicon Engine.
Computer History Museum (n.d.c) '1954: Silicon transistors offer superior operating characteristics', The Silicon Engine.
Computer History Museum (n.d.d) '1959: Invention of the "planar" manufacturing process', The Silicon Engine.
Computer History Museum (n.d.e) '1959: Practical monolithic integrated circuit concept patented', The Silicon Engine.
Computer History Museum (n.d.f) '1960: Metal oxide semiconductor (MOS) transistor demonstrated', The Silicon Engine.
Computer History Museum (n.d.g) '1963: Complementary MOS circuit configuration is invented', The Silicon Engine.
Computer History Museum (n.d.h) '1965: "Moore's Law" predicts the future of integrated circuits', The Silicon Engine.
Courtland, R. (2011) 'Intel's new transistors enter the third dimension', IEEE Spectrum, 4 May.
Dennard, R.H., Gaensslen, F.H., Yu, H.-N., Rideout, V.L., Bassous, E. and LeBlanc, A.R. (1974) 'Design of ion-implanted MOSFET's with very small physical dimensions', IEEE Journal of Solid-State Circuits, 9(5), pp. 256–268.
Directive (EU) 2024/1799 of the European Parliament and of the Council of 13 June 2024 on common rules promoting the repair of goods and amending Regulation (EU) 2017/2394 and Directives (EU) 2019/771 and (EU) 2020/1828 (2024) Official Journal of the European Union, L, 2024/1799, 10 July.
Esmaeilzadeh, H., Blem, E., St. Amant, R., Sankaralingam, K. and Burger, D. (2011) 'Dark silicon and the end of multicore scaling', in Proceedings of the 38th Annual International Symposium on Computer Architecture (ISCA '11). New York: ACM, pp. 365–376.
European Commission (2026) Proposal for the Chips Act 2.0, 3 June.
Forti, V., Baldé, C.P., Kuehr, R. and Bel, G. (2020) The global e-waste monitor 2020: quantities, flows and the circular economy potential. Bonn, Geneva and Rotterdam: United Nations University, United Nations Institute for Training and Research, International Telecommunication Union and International Solid Waste Association.
Gartner (2026a) 'Gartner forecasts worldwide semiconductor revenue to exceed $1.3 trillion in 2026', Gartner Newsroom, 8 April.
Gartner (2026b) 'Gartner forecasts worldwide semiconductor revenue to reach $1.6 trillion in 2026', Gartner Newsroom, 24 August.
Hisamoto, D., Lee, W.-C., Kedzierski, J., Takeuchi, H., Asano, K., Kuo, C., Anderson, E., King, T.-J., Bokor, J. and Hu, C. (2000) 'FinFET – a self-aligned double-gate MOSFET scalable to 20 nm', IEEE Transactions on Electron Devices, 47(12), pp. 2320–2325.
IEA (2026) Key questions on energy and AI. Paris: International Energy Agency, 16 April.
Infosys Knowledge Institute (2025) Semiconductor industry outlook 2025. Bangalore: Infosys.
Intel Corporation (2011) 'Intel reinvents transistors using new 3-D structure', Intel Corporation, 4 May.
Intel Corporation (2025) 'Intel and Trump Administration reach historic agreement to accelerate American technology and manufacturing leadership', Exhibit 99.1 to Form 8-K, 22 August.
Intel Corporation (n.d.) 'Moore's Law', Intel.
Lazenby, O. (2026) 'Intel begins tool move-in at Fab 62 as 14A customer window and tax credit deadline converge', Tech Times, 22 October.
Lécuyer, C. (2006) Making Silicon Valley: innovation and the growth of high tech, 1930–1970. Cambridge, MA: MIT Press.
Lockhart de la Rosa, C.J. and Kar, G.S. (2025) 'Introducing 2D-material based devices in the logic scaling roadmap', imec, 16 January. 
Mack, C.A. (2011) 'Fifty years of Moore's law', IEEE Transactions on Semiconductor Manufacturing, 24(2), pp. 202–207.
Marsh, A. (2024) 'The incredible story behind the first transistor radio', IEEE Spectrum, 30 September.
Mathieu, E. (2024) 'Moore's law has accurately predicted the progress in transistor counts over the last 50 years', Our World in Data, 15 April.
Moore, G.E. (1965) 'Cramming more components onto integrated circuits', Electronics, 38(8), pp. 114–117.
Noack, M. (2016) 'Chronicling the dirty side of "Techville"', Mountain View Voice, 30 August.
Nobel Prize Outreach (2026a) 'The Nobel Prize in Physics 1956', NobelPrize.org.
Nobel Prize Outreach (2026b) 'The Nobel Prize in Physics 2000', NobelPrize.org.
NVIDIA (2022) 'NVIDIA announces Hopper architecture, the next generation of accelerated computing', NVIDIA Newsroom, 22 March.
NVIDIA (2024) 'NVIDIA Blackwell platform arrives to power a new era of computing', NVIDIA Newsroom, 18 March.
Pangrle, B. (2026) 'TSMC Tech Symposium 2026, by the numbers', Semiconductor Engineering, 27 April.
Regulation (EU) 2023/1781 of the European Parliament and of the Council of 13 September 2023 establishing a framework of measures for strengthening Europe's semiconductor ecosystem and amending Regulation (EU) 2021/694 (Chips Act) (2023) Official Journal of the European Union, L 229, 18 September, pp. 1–53.
Reuters (1996) 'Celebrating 50 years of the Information Age', The Christian Science Monitor, 9 February.
Riordan, M. and Hoddeson, L. (1997) Crystal fire: the birth of the information age. New York: W.W. Norton.
Robinson, D. (2026) 'Intel bit off more than it could chew with 18A process node', The Register, 3 June.
RTÉ (2026) 'ASML lifts 2026 forecast as surging AI demand boosts new orders for chip equipment'
Samsung Electronics (2022) 'Samsung begins chip production using 3nm process technology with GAA architecture', Samsung Global Newsroom, 30 June.
ScienCentral and American Institute of Physics (1999a) 'Deciding to share', Transistorized! PBS Online.
ScienCentral and American Institute of Physics (1999b) 'The first silicon transistor', Transistorized! PBS Online.
Tanner, B. (2026) 'Gartner predicts worldwide semiconductor revenue to exceed US$1.3 trillion in 2026', Intelligent CIO, 13 April.
Trader, T. (2016) 'Transistors won't shrink beyond 2021, says final ITRS report', HPCwire, 28 July.
TrendForce (2026a) 'Global foundry revenue approaches US$53.49 billion in 2Q26 as SMIC narrows market share gap with Samsung, says TrendForce', TrendForce, 9 September.
TrendForce (2026b) 'TSMC CoWoS supply-demand gap reportedly seen narrowing from 20% to 10% by end-2026', TrendForce News, 15 June.
TSMC (n.d.) '2nm technology', TSMC.
Watzinger, M., Fackler, T.A., Nagler, M. and Schnitzer, M. (2020) 'How antitrust enforcement can spur innovation: Bell Labs and the 1956 Consent Decree', American Economic Journal: Economic Policy, 12(4), pp. 328–359.
WSTS (2025) 'Global semiconductor market approaches $1T in 2026', World Semiconductor Trade Statistics, December.
WSTS (2026) 'Global semiconductor market surges beyond $1.5T 2026', World Semiconductor Trade Statistics, 2 June.

research and referencing was done with local alliterated LLM with auto log clearance so prompt history is unavailable
