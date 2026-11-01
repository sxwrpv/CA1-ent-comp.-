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
Scaling is expected to continue at greater cost. TSMC’s A16 process, featuring backside power delivery, reportedly shifted from late 2026 to 2027; A14 is targeted for 2028 (SemiEngineering, 2026). Imec places CFETs at the A7 generation and two-dimensional channel materials later, with contacts, doping and integration still unresolved (imec, n.d.)
As chips approach the reticle limit, chiplets, high-bandwidth memory and advanced packaging offer further gains. Capacity remains a constraint for technologies such as TSMC’s 5.5-reticle CoWoS (SemiEngineering, 2026; TrendForce, 2026b). TSMC’s COUPE brings optical connections into packages (SemiEngineering, 2026).
Neuromorphic photonic systems still require electronic control and conversion; their energy advantages over GPUs lack comparable benchmarking (Bile, 2026). IBM’s and Google’s quantum milestones around 2030 remain company targets, not delivered results (Andes Qubit, 2026).
6.  Business Viewpoint
7. Ethical Reflection and Improvements
Conclusion: 
References
