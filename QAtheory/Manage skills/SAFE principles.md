## 1. Take an economic view

- achieving the shortest sustainable lead time with the best quality and value;
- Deliver Early and Often;
- Understand Solution Economic Trade-Offs
    - Identifies five considerations that affect these decisions:  
        A. Development expense – the cost of labor and materials required to implement a capability Lead time – the time needed to implement the capability (described as ‘Cycle time’ in Reinertsen’s work)  
        B. Product cost – the manufacturing cost (of goods sold) and/or deployment and operational costs  
        C. Value – the economic worth of the capability to the business and the customer  
        D. Risk – the uncertainty of the solution’s technical or business success  
        ![Principle-1_F4_web-768x587.webp](file:///C:/Users/Artsemi_Vadalazau/.config/joplin-desktop/resources/6fc242fc30d24a58b98dead80f47ed58.webp)
- Sequence Jobs for Maximum Benefit
    - To minimize the cost of delay (COD), jobs are pulled into implementation based on Weighted Shortest Job First (WSJF). WSJF prioritizes the backlog to ensure the highest value is delivered in the shortest lead time  
        ![WSJF_F03-WP.webp](file:///C:/Users/Artsemi_Vadalazau/.config/joplin-desktop/resources/c1ea10739cf045bd9797f99870f63c02.webp)
- Practices Provide the Form. People Make the Decisions

## 2. Apply systems thinking

- Team members must understand clearly the boundaries of the system, what it is, and how it interacts with the environment and the systems around it
- Optimizing a component does not optimize the system.
- Components can become selfish and hog the resources—computing power, memory, electrical power, whatever—that other elements need
- For the system to behave well as a system, intended behavior and some higher-level understanding of its architecture (how the components work together to accomplish the aim of the system) must be understood. Intentional design is fundamental to systems thinking
- The value of a system passes through its interconnections. Those interfaces—and the dependencies they create—are critical to providing ultimate value
- Continuous attention to those interfaces and interactions is vital. A system can evolve no faster than its slowest integration point.
- The faster the full system can be integrated and evaluated, the faster the system knowledge grows
- The Enterprise Building the System Is a System, Too
- Building complex systems is a social endeavor. Therefore, leaders must cultivate an environment where people collaborate on the best way to build better systems.
- Suppliers and customers are integral to the development value stream. They must be treated as partners, based on a long-term foundation of trust.
- Optimizing a component does not optimize the system in this case, either. Therefore optimizing local teams or functional departments does not enhance the flow of value through the enterprise. And as with physical systems, the value of the system passes through its interfaces here too.
- Accelerating flow delivery requires eliminating silos and creating cross-functional organizations, such as Agile Release Trains (ARTs) and Solution Trains.
- Understand and Optimize the Full Development Value Stream
- One essential process is value stream mapping, a systematic way to view all the steps required to produce value. This allows leaders to quickly recognize that the actual value-added processing steps—creating code and components, deployment, validation, etc.—consume only a small portion of the total time-to-market. This recognition drives these leaders to constantly focus on the delays between steps  
    ![2-Apply-Systems-Thinking_F03_WP.webp](file:///C:/Users/Artsemi_Vadalazau/.config/joplin-desktop/resources/71e59af9d9274877b349412748d84c87.webp)
- Only Management Can Change the System
    - Exhibit and teach systems thinking and Lean-Agile values, principles, and practices
    - Engage in solving problems and eliminating roadblocks and ineffective internal systems
    - Apply and teach root-cause analysis and corrective action techniques
    - Collaborate with the teams to reflect at key Milestones and identify and address shortcomings
    - Take a long-term view, investing in enabling capabilities such as infrastructure, practices, and tools and training that lead to faster value delivery and higher quality and productivity
    - Foster a Continuous Learning Culture that includes relentless improvement in the application of systems thinking

## 3. Assume variability; preserve options

- Preserve Options with Set-Based Design
    - We are operating early in the ‘cone of uncertainty’ and attempting to force certainty by freezing requirements and design. The bigger and more technically innovative the system is, the higher the odds are that the agreed starting point was not the best one
    - developers cast a wider design net initially, considering multiple design choices at the start. After that, they continuously evaluate economic and technical trade-offs—typically as exhibited by the objective evidence presented at integration-based learning points. Then they eliminate the weaker options over time and ultimately converge on a final design, based on the knowledge gained to that point

## 4. Build incrementally with fast, integrated learning cycles

- Rather than pick a single requirements-and-design choice early on - assuming that it’s feasible and will provide fitness for purpose - a range of requirements and design options (Principle #3) are considered while building the solution incrementally in a series of short timeboxes. Each results in an increment of a working system that can be evaluated. Subsequent timeboxes build on the previous increments, and the solution evolves until it’s released. The knowledge gained from integration points is not solely to establish technical viability. Many integration points can also serve as minimum viable solutions or prototypes for testing the market, validating usability, and gaining objective customer feedback. Where necessary, these fast feedback points allow teams to pivot to an alternate course of action, one that should better serve the needs of the intended customers.
- Faster Learning through Faster Cycles Integration points are an example of Shewhart’s plan-do-check-adjust cycle and are the mechanism for controlling the variability of solution development. The more frequent the points, the faster the learning. In complex systems development, local integration points are used to assure that each system element or capability is meeting its responsibilities to contribute to the overall Solution Intent. These local points must then be integrated at the next higher system level. The larger the system, the more such integration levels exist. Solution designers recognize that the top-level, least-frequent integration point provides the only true measure of system progress, and they work to create these points as frequently as possible. All stakeholders understand that when the timing of integration points slips, the project is in trouble. But even then, this knowledge helps spark the necessary adjustments to scope, technical approach, cost, or the delivery timing needed to redirect the project to meet revised expectations.

## 5. Base milestones on objective evaluation of working systems

- The cause of the problem is the failure to recognize the four critical errors in the assumption that phase gates reveal real progress and thus mitigate risk:
    - Centralizing requirements and design decisions in siloed functions that do not actually build the system. Forcing too-early design decisions and false-positive feasibility
    - An early choice is made for the best-known option at that time. Development proceeds under the assumption that everything is on track. Later it’s discovered that the chosen path is not feasible (Principle #3)
    - Assuming a point solution exists and can be built correctly the first time. This ignores the variability inherent in the process and provides no legitimate outlet for it.
    - Variability will find a way to express itself. Making up-front decisions creates large batches of requirements, code, and tests, and long queues. This leads to large-batch handoffs and delayed feedback (Principle #6)
- Base Milestones on Objective Evidence

## 6. Visualize and limit WIP, reduce batch sizes, and manage queue lengths

- To achieve the shortest sustainable lead time, Lean enterprises strive for a state of continuous flow, which allows them to move new system features quickly from ‘concept to cash’. Accomplishing flow requires eliminating the traditional start-stop-start project initiation and development process, along with the incumbent phase gates that hinder flow (see Principle #5 and Lean Budgets). Three primary keys to achieving flow are:
    - Visualize and limit work in process (WIP)
    - Reduce the batch sizes of work items
    - Manage queue lengths
- Having too much WIP confuses priorities, causes frequent context switching, and increases overhead. It overloads people, scatters focus on immediate tasks, reduces productivity and throughput, and increases wait times for new functionality. Like a highway at rush hour, there is simply no upside to having more work in a system than the system can handle. The first step to correct the problem is to make the current WIP visible to all stakeholders. A Kanban board is a simple way of doing that
- The next step is to start balancing the amount of WIP against the available development capacity. This is done by establishing - and continually adjusting - WIP limits for the relevant states. Simply, when any workflow state reaches its WIP limit, no new work is taken on. This matches demand to capacity and increases flow through the system.
- decrease the batch sizes of the work - the requirements, designs, code, tests, and other work items that move through the system. Small batches go through the system more quickly and with less variability, which fosters faster learning. The reason for the faster speed is obvious.
- The third method of achieving flow is to manage queue lengths.
    - Keep team and program backlogs short and largely uncommitted. This allows new, higher priority work to enter and leave the system with less wait time.
    - Establish WIP limits for each process step. This means that the length of the queue in front of any one state is limited to the WIP limit.
    - Be especially careful of large, long-term commitments. It’s always tempting to look into the future and make a long-range commitment which seems to satisfy the need for certainty about the future. But very long-term commitment increases the response time for new opportunities. In other words, every long-term commitment decreases the agility of the enterprise.

## 7. Apply cadence, synchronize with cross-domain planning

- Cadence is a rhythmic pattern of events that provides the steady heartbeat of the development process. It makes routine everything that can be routine, so developers can focus on managing the variable part of solution development.
- Synchronization allows multiple solution perspectives to be understood, resolved, and integrated at the same time.

|Principles of Flow: Cadence|SAFe Practices|
|---|---|
|F5: Use a regular cadence to limit the accumulation of variance|Planning at regular PI intervals limits variances to a single PI timebox, increasing Agile Release Train (ART) and Solution Train predictability|
|F6: Provide sufficient capacity margin to enable cadence|In order to reliably meet PI objectives, the Innovation and Planning (IP) iteration has no planned scope and provides a schedule margin (buffer). In addition, planned-for but uncommitted objectives provide capacity margin (scope buffer). Together, they offer a way to reliably meet PI goals|
|F7: Use cadence to make waiting times predictable|If a Feature doesn’t make it into a PI but remains a high priority, its delivery can be scheduled for the next PI (or another scheduled, frequent release). This avoids the temptation to load excess Work in Process (WIP) into the current increment|
|F8: Use a regular cadence to enable small batch sizes|Short iterations help control the number of Stories in the iteration batch. Feature batch sizes are controlled by short PIs and frequent releases, providing high system predictability and throughput|
|F9: Schedule frequent events using a predictable cadence|PI planning, System Demos, Inspect and Adapt (I&A), ART Sync, Iteration Planning, backlog refinement, and architecture discussions are examples of things that benefit from frequent events. Each event needs to process only a small batch of new information. Cadence helps lower the transaction costs of these events|
|F10: Exploit economies of scale by synchronizing work from multiple projects|Individual Agile Teams are aligned to common iteration lengths. Work is synchronized by system and solution demos. Portfolio business and Enabler Epics drive common infrastructure and Customer utility|
|F11: Capacity margin enables synchronization of deliverables|The Innovation and Planning (IP) iteration enables the final PI system demo, and solution demo to occur without taking velocity away from ARTs or Solution Trains|
|F12: Use synchronized events to facilitate cross-functional trade-offs|ART and Solution Train events synchronize customer feedback and enable resource and budget adjustments, mission alignment, continuous improvement, and program oversight and governance. They also drive collaboration and team building|
|F13: To reduce queues, synchronize the batch size and timing of adjacent processes|Teams are aligned to common timeboxes and similar batch sizes. The ART and solution system teams support integration on a regular cadence. To facilitate the rapid delivery of new ideas, backlogs are kept short and uncommitted|
|F14: Apply nested cadence harmonic multiples to synchronize work|Teams integrate and evaluate on iteration boundaries (at least). ARTs and Solution Trains evaluate on PI boundaries|

![7-Apply-Cadence_F04_WEB.webp](file:///C:/Users/Artsemi_Vadalazau/.config/joplin-desktop/resources/140ca75dc5c44d74982634aba23c9bc2.webp)

## 8. Unlock the intrinsic motivation of knowledge workers

- Leverage the Systems View Before
    - Communicate across functional boundaries
    - Make decisions based on an understanding of the economics
    - Receive fast feedback about the efficacy of their solution
    - Participate in continuous, incremental learning and mastery
    - Participate in a more productive and fulfilling solution development process —one of the most powerful motivations of all
- Understand the Role of Compensation
    - If you don’t pay enough, people won’t be motivated.
    - But after a point, money is no longer a motivator.
- Provide Autonomy with Purpose, Mission, and Minimum Possible Constraints
    - The mission, a general goal and strategic direction, and a strong vision
    - Little, minimal, or even no specific work or project plans
    - Challenging requirements, along with the minimum possible constraints as to how teams meet these requirements
- Create an Environment of Mutual Influence
    - Disagree where appropriate
    - Advocate for the positions they believe in
    - Make their needs clear and push to achieve them
    - Enter into joint problem-solving with management and peers
    - Negotiate, compromise, agree, and commit

## 9. Decentralize decision-making

- Centralize Strategic Decisions
    - Infrequent – Made infrequently, these decisions typically are not urgent, and deeper consideration is appropriate (ex., product strategy, international expansion).
    - Long-lasting – Once made, these decisions are unlikely to change at least in the short term (e.g., commitment to a standard technology platform, commitment to organizational realignment around Value Streams).
    - Provide significant economies of scale – These choices deliver large and broad economic benefits (e.g., a common way of working, standard development languages, standard tooling, offshoring). Leadership is charged with making these types of decisions, supported by the input of those stakeholders who are affected by the results.
- Decentralize Everything Else
    - Frequent – The problems addressed by decentralized decisions are recurrent and common (e.g., Team and Program Backlog prioritization, real-time Agile Release Train [ART] scoping, response to defects and emerging issues).
    - Time-critical – Delaying these types of decisions comes with a high cost of delay (e.g., point releases, customer emergencies, dependencies with other teams).
    - Require local information – These decisions need specific local context, whether it be technology, organization, or specific customer or market impact (e.g., shipping a release to a specific customer, resolve a significant design problem, self-organization of individuals and teams to an emerging challenge).
- A Lightweight Thinking Tool for Decision-Making

![9-Decentralize-Decision-Making_F01_WP.webp](file:///C:/Users/Artsemi_Vadalazau/.config/joplin-desktop/resources/2071f10b955f4cec83a1207164f249af.webp)

## 10. Organize around value

- The Network optimizes the flow of value by:
    - Reducing handoffs and delays between functional areas, reducing time to market
    - Bringing together all the research, development, deployment, and service personnel needed to offer whole product solutions
    - Providing intense customer focus across all disciplines for each product and service type
    - Measuring success via meaningful, outcome-based key performance indicators
    - And perhaps most importantly, the Network can rapidly reorganize as necessary to support emerging opportunities and competitive threats
- How SAFe Organizes Around Value
    - ABuild Technology Portfolios of Development Value Streams
        - Precisely specify value by specific product Identify the value stream for each product
        - Make value flow without interruptions Let the customer pull value from the producer
        - Pursue perfection
    - Organizing a portfolio this way offers many benefits:
        - Helps assure customer and product focus across the entire portfolio
        - Aligns strategy to execution by bringing visibility to all the work
        - Provides the basis for Lean Budgets, which eliminates the friction and cost accounting overhead of traditional project-based work
        - Supports measuring success via outcome-based key performance indicators (KPIs)
        - Improves workflow with smaller batch sizes
- Realize Value Streams with Product Focused Agile Release Trains
- Scaling the ART into Solution Trains
- Form Cross-Functional Agile Teams That Directly Deliver Value
- Reorganizing around Value

---

[source](https://www.scaledagileframework.com/ "https://www.scaledagileframework.com/")