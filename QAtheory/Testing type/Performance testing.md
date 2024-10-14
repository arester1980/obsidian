1. Response time
2. Throughput
3. Environment
4. Each process time
5. Interoperability
6. ETL (extract - transfer - load data from one DB to other)
7. Increasing Load

### Start from:

- do we have criteria of perfomance? - often answer "No", but customer can said: "Let's try what happen if 1.000.000 users try to login"
- what we should test (components, system, etc.)
- normal and maximum count for users / instances
- what the architecture of system that will be tested
- what scenario of use each components of system (20% sign in, 40% search, 10% log out and etc.)
- what user's scenario
- what time requirement for each components of system?

### Types:

- [Load testing](joplin://2f6dd42dcb5e46c9ac18aec3643bfe97) - скорость при возрастающей нагрузке
- стабильность / stability - работа на среденей нагрузке длительное время
- отказоустойчивость / failover - возможность самовостанавливаться
- восстановление / recovery - как быстро восстановится
- [Stress testing](joplin://b9fb83a33d644e8d8518a6021b1519b5) - критическая высокая нагрузка
- объемное / volume - увеличение БД в 100 раз
- масштабируемость / scalability - поведение при увеличении числа пользователей
- потенциальных возможностей / capacity - сколько может работать в системе без проблем
- конфигурационное / configuration - как заставить работать быстрее
- сравнения / compare - какое обороудование и ПО выбрать
- _Spike-тестирование_ — это подтип стресс-тестирования. В нем фокус смещен на производительность приложения под огромными нагрузками в течение коротких периодов времени. Такие перепады создаются либо между периодами обычной нагрузки приложения в продакшене (продакшен-среда имитируется), либо вообще без «фоновой» нагрузки.

see also [Perfomance Testing](joplin://e5546d41b6b04420aba62adeb138b46c)

### Tools:

- Gatling
- JMETER
- THE GRINDER
- LOCUST
- WEBLOAD
- Chrome Dev tools
- Google Lighthouse / Audits
- Google pagespeed insights
- Webpagetest
- Sitespeed.io
- Apache Jmeter

---

Way of increase loading speed:

- minimize of HTML / JS code (see [minifycode](http://minifycode.com "http://minifycode.com"))
- optimize Size/Volume of pics
- enable compression not only HTML (availbale for NGINX)
- check out cashing (what and how long save)
- parralalize loading (10 threads of loading instead 6 threads)
- add async to code for non-cricical JS scripts
___
> **Performance of a software system** - is its quality characteristics that indicates system’s ability to be as powerful (capable), fast, reliable, and scalable as required

> **Performance analysis** - is conducted to find root causes of observed performance issues. It usually comes to identification of performance bottlenecks: phenomenon where the performance of an entire system is limited by a single or limited number of components or resources.

#### Performance testing is to be carried out to answer the questions like:

1. Would a system perform well under certain workload?
2. Would system work stably under load for a long period of time?
3. Would it be possible to scale the system up if load increases in future?
4. How many hardware resources would be required to support expected load?

---

### Terms:

|Term|Description|
|---|---|
|Response time|It is time a system takes to fulfill client’s request = This is measure of how fast the system is|
|Capacity|It’s the highest level of load a system can take and handle without significant increase in response time and issues with stability = This is measure of how powerful the system is|
|Stability|It is a property that indicates system's ability to maintain its level of operation / Reliability: stability in predefined conditions (load) proven for a specific period = Extended resistance to failure: stability beyond stated conditions and/or beyond stated period|
|Scalability|It is a property that indicates system's ability to be readily enlarged = That means that capacity of ideally scalable system should increase proportionally to the resources allocated for that system|
|[Load testing](joplin://2f6dd42dcb5e46c9ac18aec3643bfe97) - скорость при возрастающей нагрузке||
|стабильность / stability - работа на среденей нагрузке длительное время||
|отказоустойчивость / failover - возможность самовостанавливаться||
|восстановление / recovery - как быстро восстановится||
|[Stress testing](joplin://b9fb83a33d644e8d8518a6021b1519b5) - критическая высокая нагрузка||
|объемное / volume - увеличение БД в 100 раз||
|масштабируемость / scalability - поведение при увеличении числа пользователей||
|потенциальных возможностей / capacity - сколько может работать в системе без проблем||
|конфигурационное / configuration - как заставить работать быстрее||
|сравнения / compare - какое обороудование и ПО выбрать||
|_Spike-тестирование_ — это подтип стресс-тестирования. В нем фокус смещен на производительность приложения под огромными нагрузками в течение коротких периодов времени. Такие перепады создаются либо между периодами обычной нагрузки приложения в продакшене (продакшен-среда имитируется), либо вообще без «фоновой» нагрузки.||

---

### Server-side

> aims on measuring the backend performance of applications end-to-end as well as individual components performance

|Test type|Load Model|Purpose|Outcome|
|---|---|---|---|
|capacity|Gradual load increase|Get saturation point and(or) point of instability of the system for defined scenario|Number of requests at saturation|
||Duration will be defined experimentally||Response time of requests at saturation|
||||Behavior of the system before saturation and after|
|response time|Stable load (expected load, production load, or some percentage of saturation load - usually 80%)|Check system behavior under stable load|Response time of user transactions for current release|
||1 hour duration|Measure response time for user transactions under defined stable load|Throughput level of user transactions (RPS)|
|||Compare current results with previous ones or get new baseline|Deviation of response time and throughput in comparison with previous release or new baseline metrics|
|stability/longevity|Stable load (expected load, production load, or some percentage of saturation load - usually 80%)|Check system stability under stable load during prolonged period|Status of system stability during prolonged period|
||4-12 hours duration|Check if the system has memory leaks or bottlenecks that can be observed after prolonged period of system running||
|UI test|1 UI user|Measure browser metrics for complete page loads and user actions|Baseline of First Contentful Paint, Largest Contentful Paint, Cumulative Layout Shift, First Visual Change, Last Visual Change, Total Blocking Time metrics values for 1 user|
|Mobile application UI test|1 UI user|Measure mobile metrics for complete page loads and user actions|Baseline of user action response time, frames per second (FPS), render frame jank, hardware metrics for 1 user|
|scalability - stress tests to verify system is able to sustain defined stressful conditions|scalability _vertical_ - to identify optimal configuration|scalability _horizontal_ - to assess the ability of system to scale according to increased load||

---

### Client-side (or UI)

_Client side test is conducted under 1 user optionally includes backend performance tests to assess its influence on UI rendering speed_

---

**System and application monitoring** - includes monitoring of system components metrics like CPU, memory, disk, network for observability of system health during the test. Additionally as part of application monitoring application logs analysis on component level can be done in case if logs are accessible. Results of monitoring and logs analysis are considered in root cause investigation.  
**Test data management** - includes building and implementing test data management strategy by creating additional scripts, code to generate prod-like or agreed amount of data in storage system components as well as building mechanism of importing, updating, clean-up data to keep tests data in certain state. Enabling test data management allows to reach tests repeatability under the same conditions and thus ensure proper comparison of results from test to test.

## Important metrics to measure

- [**First Contentful Paint (FCP):**](https://web.dev/fcp/ "https://web.dev/fcp/") measures the time from when the page starts loading to when any part of the page's content is rendered on the screen. (lab, field)
- [**Largest Contentful Paint (LCP):**](https://web.dev/lcp/ "https://web.dev/lcp/") measures the time from when the page starts loading to when the largest text block or image element is rendered on the screen. (lab, field)
- [**First Input Delay (FID):**](https://web.dev/fid/ "https://web.dev/fid/") measures the time from when a user first interacts with your site (when they click a link, tap a button, or use a custom, JavaScript-powered control) to the time when the browser is actually able to respond to that interaction. (field)
- [**Interaction to Next Paint (INP):**](https://web.dev/inp/ "https://web.dev/inp/") measures the latency of every tap, click, or keyboard interaction made with the page, and—based on the number of interactions—selects the worst interaction latency of the page (or close to the highest) as a single, representative value to describe a page's overall responsiveness. (lab, field)
- [**Time to Interactive (TTI):**](https://web.dev/tti/ "https://web.dev/tti/") measures the time from when the page starts loading to when it's visually rendered, its initial scripts (if any) have loaded, and it's capable of reliably responding to user input quickly. (lab)
- [**Total Blocking Time (TBT):**](https://web.dev/tbt/ "https://web.dev/tbt/") measures the total amount of time between FCP and TTI where the main thread was blocked for long enough to prevent input responsiveness. (lab)
- [**Cumulative Layout Shift (CLS):**](https://web.dev/cls/ "https://web.dev/cls/") measures the cumulative score of all unexpected layout shifts that occur between when the page starts loading and when its lifecycle state changes to hidden. (lab, field)
- [**Time to First Byte (TTFB):**](https://web.dev/ttfb/ "https://web.dev/ttfb/") measures the time it takes for the network to respond to a user request with the first byte of a resource. (lab, field)
- [**Top Metrics You Need to Understand When Measuring Front-end Performance**](https://blog.openreplay.com/top-metrics-you-need-to-understand-when-measuring-front-end-performance "https://blog.openreplay.com/top-metrics-you-need-to-understand-when-measuring-front-end-performance")

## Custom metrics

- [User Timing API](https://w3c.github.io/user-timing/ "https://w3c.github.io/user-timing/")
- [Long Tasks API](https://w3c.github.io/longtasks/ "https://w3c.github.io/longtasks/")
- [Element Timing API](https://wicg.github.io/element-timing/ "https://wicg.github.io/element-timing/")
- [Navigation Timing API](https://w3c.github.io/navigation-timing/ "https://w3c.github.io/navigation-timing/")
- [Resource Timing API](https://w3c.github.io/resource-timing/ "https://w3c.github.io/resource-timing/")
- [Server timing](https://w3c.github.io/server-timing/ "https://w3c.github.io/server-timing/")

---

**TaaS** - model of work team can consists of Core and Flex team. Core team is named resources tied to the project, Flex team is unnamed resources that can be onboarded on demand without binding to location.

**Application performance lies on 3 pillars:**

1. Testing:

- analyze user flows to build representative load models
- develop performance test scenarios (backend, client-side, mobile incl. native apps)
- report on performance tests execution results
- highlight potential zones of interest for performance analysis

2. Analysis:

- analyze architecture to identify potential points of interest
- analyze individual system component performance
- conduct deep root-cause analysis for issues and bottlenecks discovered during testing
- propose practical improvements and fixes

3. Engineering:

- identify product quality attributes covered by metrics and measurements
- establish process of performance issues prevention and early identification
- contribute to scaling and high-availability strategy and implementation
- facilitate configuration of effective monitoring and alerting systems

#### PTaaS Service includes

|preparation & scripting|system baselining|perfomance analysis|continuous support|
|---|---|---|---|
|Create load model based on application usage patterns. Develop backend test scripts using tool of choice (jMeter or Gattling). Develop frontend set of checks|Pre-execution to assess that environment is ready to accept the load. Whole set of tests execution (Capacity, Longevity, Response time). Establishing/adjusting a base-line for continuous execution|Analyze reasons of performance failures. Identify application improvement areas. Help in configuration of effective system and application monitoring and alerting. Help in establishing test data management practices|Regular test execution (response time tests). Update of test scripts according to product increments|

### PTaaS Service can be use:

| Case A (Flex team)                                                                                                                     | Case B (Core and Flex team) - Flex team in this case covers the scope related to performance testing and elimination of technical debt, while Core team conduct deep analysis and retain project specific knowledge |                                                                                                                                    |
| -------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------- |
| Info                                                                                                                                   | Projects looking for performance testing only (w/o analysis) should consider subscription based models to reduct the overall cost of implementation and execution to absolute minimum                               | Project looking for a performance testing and performance analysis to be covered as a part of engagement                           |
|                                                                                                                                        | Initial system performance baselining with capacity, longevity and response time tests, including web UI tests                                                                                                      | Test approach working out                                                                                                          |
|                                                                                                                                        | Regular response time test executions handled by request within 24 hours or less of timeframe                                                                                                                       | Scripts developing (UI, backend, mobile)                                                                                           |
|                                                                                                                                        | Reports after test execution: Reevaluation of system’s baseline once per every major release, but not more then once per month for weekly based execution, and once per quarter for monthly+ based executions       | Testing framework/infrastructure preparation (installation and configuring software)                                               |
|                                                                                                                                        | Update of test scenarios time for up to 16 hours per month in case of weekly, bi-weekly and monthly tests, and 32 hours per execution in case of quarterly tests, this quota can be increased by agreement          | Test data management implementation                                                                                                |
|                                                                                                                                        | Brief results overview just after tests are done                                                                                                                                                                    | 3rd party mocking                                                                                                                  |
|                                                                                                                                        | Comprehensive version in PDF in 1-2 business days after test execution                                                                                                                                              | Hardware/application monitoring setup (if required)                                                                                |
|                                                                                                                                        | All infrastructure costs to run performance tests                                                                                                                                                                   | CI pipeline creation with quality gates                                                                                            |
|                                                                                                                                        | Regular response time test duration is scoped for 1 hour of active testing                                                                                                                                          | Running set of baseline tests: backend: capacity, response time and longevity / UI: lighthouse, sitespeed / Mobile: apptim, appium |
|                                                                                                                                        | Every system baselining scoped for 2-3 days of active testing                                                                                                                                                       | Test results and root cause analysis                                                                                               |
|                                                                                                                                        |                                                                                                                                                                                                                     | Preparing detailed test report                                                                                                     |
|                                                                                                                                        |                                                                                                                                                                                                                     | Preparing knowledge transfer documentation                                                                                         |
|                                                                                                                                        |                                                                                                                                                                                                                     | Making demo of results and KT to the project team                                                                                  |
|                                                                                                                                        |                                                                                                                                                                                                                     | Every system baselining scoped for 2-3 days of active testing                                                                      |
| _Billing Service work is calculated in Service Points. Service point is 1 hour of effective work to cover defined scope. For example:_ |                                                                                                                                                                                                                     |                                                                                                                                    |
| _- Develop a small performance flow (number of requests < 5) = 5 SPs_                                                                  |                                                                                                                                                                                                                     |                                                                                                                                    |
| _- Fix issues small performance flow without changing flow itself = 3 SPs_                                                             |                                                                                                                                                                                                                     |                                                                                                                                    |
| _- Investigate failures during performance tests execution = 1 SPs_                                                                    |                                                                                                                                                                                                                     |                                                                                                                                    |

---

# Flow

## Creating Load Models

gather and process all required information about the project:

- Business purpose of the project
- Architecture of the application
- User scenarios (to be scripted for load testing)
- Performance requirements (if exists)
- Test data for scenarios
- Test and production environment description

> Idea with API calls was presented in a right way (not all HTTP requests from a page, but only those which are dynamic REST|AJAX calls; all static resources should also be loaded from a page in load test in majority of cases, but it could be done automatically using in-built features of load testing tools). One 'branch' of scenarios with chair is presented correctly. However, if you'll calculate total % of users who proceeded to checkout it will be 0,5 * 0,3 = 0,15 (30% of 50% -> 15%). What should be done is adding another 'branch' for scenario, leading from 'add table to cart' directly to 'open cart' with 15% chance. But generally it's a matter of how you represent it and could be arguable.  
> [Load Model.pdf](file:///C:/Users/Artsemi_Vadalazau/.config/joplin-desktop/resources/f0725760272b4d75a248855b05276c3a.pdf "file:///C:/Users/Artsemi_Vadalazau/.config/joplin-desktop/resources/f0725760272b4d75a248855b05276c3a.pdf")

#### Get answer to the next quiestions:

- do we have criteria of perfomance? - often answer "No", but customer can said: "Let's try what happen if 1.000.000 users try to login"
- what we should test (components, system, etc.)
- normal and maximum count for users / instances
- what the architecture of system that will be tested
- what scenario of use each components of system (20% sign in, 40% search, 10% log out and etc.)
- what user's scenario
- what time requirement for each components of system?
- #### What is the set of possible actions that a user can perform?
    
    - Connect to the home page.
    - Log on to the application.
    - Browse the product catalog.
    - Search for specific products.
    - Add products to the shopping cart.
    - Validate and place an order.
    - Log out from the application.
- #### What are user profiles for the application? Will a single user profile be enough?
    
    - Browse profile
    - Search profile
    - Place order profile
- #### What are the actions performed by a user representative of each profile?
    
    |Operation|Number of times performed in a single session|
    |---|---|
    |Connect to the home page|1|
    |Log on to the application|1|
    |Browse the product catalogue|4|
    |Search for specific products|2|
    |Add products to the shopping cart|3|
    |Validate and place order|1|
    |Log off from the application|1|
    
- #### What is the average user “think time” between actions?
    
- #### What is the expected ratio of user profile scenarios?
    
    - For instance, a typical usage pattern of an e-commerce application could be 77% of users browsing the site; 20% searching for particular products, and 3% placing an order. This is based on a conversion rate of 3 percent (your conversion rate may differ)
- #### How does the number of users logged on to your site vary with time?
    
- #### What is the maximum expected number of users logged in to your application?
    
- #### What is the duration for which the test needs to be executed?
    
    - You need to test your login mechanism to ensure that a required number of users can log in to the site within a certain period of time. This scenario can be testing in a short period of time (15-20 minutes) and the results can be extrapolated for longer periods. If 100 users can log in within 15 minutes, it can be extrapolated that 400 users can log in within an hour.
    - You may run tests continuously for an extended period of time (days, and possibly weeks) with a constant load to observe how your application performs over the long haul. This identifies slow memory leaks that only become apparent over a long period of time.

### There are 3 ways to identify set of user actions to be emulated during performance tests:

- Business critical user actions (the main reason why the application exists - e.g. if it's e-commerce, then business-critical actions are search for a product and check-out)
- Most common user actions (usually overlaps almost completely with business critical user actions)
- Performance-heavy user actions (for example, there might be an activity of generating report for a system once a day, which requires a lot of resources and potentially may make the system slower).

> All 3 types of user actions for load model **should be identified by stakeholders and subject matter experts** (Product Owners, Business Analysts for business critical and most common, architects and lead developers for performance-heavy).

---

## ! Test environment for performance testing should be as close to production environment as possibe !

Ideal situation is so-called **blue/green deployments**. In that deployment strategy there are 2 identical environments. First one (blue) acts as a test environment for currently developed version, and second (green) serves as production environment. After all tests are done on blue environmen (including performance testing), it starts acting as production (all real users are routed to it), and now green environment is a test environment for next version.  
Unfortunately in real world test environment might differ from production. Scaled down environment should preserve horizontal levels of architecture: **if production environment contains 10 web servers and 5 app servers, test environment can have reduced number of machines on every level, but you shouldn't remove the level entirely, like hosting web and app servers on the same machines**. Such scaled down environment leaves you a possibility to extrapolate results your get to the size of production environment. Testing on improperly scaled down environment (with incorrect architecture layers) is really risky and shouldn't be done.

---

## Test data

### Data used by script

Scripts should mimic real users behavior, so all interaction from scripts should be as different as real users interaction. If there is a search functionality, make search queries as diverse as in real world might be rather complicated. But these queries should be diverse enough not to trigger caching mechanisms inside the system.

### Data in the system

System speed depends a lot on data volume, so if your test system contains much less data than production system – then your test results will be wrong. Sometimes getting production data may be prohibited because of sensitive data in it, then production data should be obfuscated or the same volume of similar data should be generated for performance testing environment.

---

### Examples of metrics

- time of start request sending
- time of start reciving answer
- time of get the last bite of recive
- time between the first and the last bytes of recive

---

1. Response time
2. Throughput
3. Environment
4. Each process time
5. Interoperability
6. ETL (extract - transfer - load data from one DB to other)
7. Increasing Load

---

# Tools

- Chrome Dev tools
- Google Lighthouse / Audits
- Google pagespeed insights
- Webpagetest
- Sitespeed.io
- Apache Jmeter
- Gatling
- THE GRINDER
- LOCUST
- WEBLOAD

---

Way of increase loading speed:

- minimize of HTML / JS code (see [minifycode](http://minifycode.com "http://minifycode.com"))
- optimize Size/Volume of pics
- enable compression not only HTML (availbale for NGINX)
- check out cashing (what and how long save)
- parralalize loading (10 threads of loading instead 6 threads)
- add async to code for non-cricical JS scripts