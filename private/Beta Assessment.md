1. не понимание того, "кто я" на рынке труда, куда я хочу развиваться
2. при ответе придерживаться вопроса
3. ситуационные задачи - как в реальности
___
##### Vividus experience:
4. How do you ensure that test cases cover all requirements, including edge cases and negative scenarios?
5. Explain the process of creating guides or documentation related to complex project flows. How do you ensure that the information is accurate, up-to-date, and easily understandable?
6. How do you coordinate QA work during releases? What challenges do you typically encounter, and how do you address them?
7. Describe a situation where you had to adapt to changing environments or requirements. How did you handle the situation, and what did you learn from it?
8. Explain the purpose and structure of the `vividus.properties` file in Vividus. What are some common properties that can be configured in this file?
9. How does Vividus handle environment-specific configuration? Describe the process of setting up and using different configuration profiles for different environments (e.g., dev, staging, production).

##### Time Estimation:
10. What are the different techniques used for estimating the time required for testing activities
11. How do you account for uncertainties and risks when estimating testing time?
12. Describe a situation where your initial time estimate was significantly different from the actual time required. What did you learn from this experience?

##### ROI Calculation:
12. What factors do you consider when calculating the return on investment (ROI) for testing activities?
13. Explain the importance of ROI calculations in justifying testing efforts to stakeholders.

##### Traceability Matrix:
14. What is a traceability matrix, and why is it important in software testing?
15. Describe a scenario where a traceability matrix helped you identify gaps or inconsistencies in testing coverage.

##### Risk-Based Testing:
16. What is risk-based testing, and why is it important?
17. How do you identify and prioritize risks in software testing?
	1. Risk Identification: budget, schedule, personnel, technical issues, etc. You can use methods like brainstorming, checklists, assumption analysis, and diagramming techniques to identify risks.
	2. Risk Analysis: based on their probability of occurrence and the impact on the project if they occur.
	3. Risk Prioritization: based on their potential impact and probability. The risks that have the highest probability and impact are given the highest priority. Create risk matrix

|                   | Low Impact  | Medium Impact  | High Impact    |
| :---------------- | :---------- | :------------- | :------------- |
| Low Likelihood    | Low Risk    | Medium Risk    | High Risk      |
| Medium Likelihood | Medium Risk | High Risk      | Very High Risk |
| High Likelihood   | High Risk   | Very High Risk | Extreme Risk   |
	4. Risk Response Planning: Develop strategies to manage and mitigate the high-priority risks. These strategies could include risk avoidance, risk reduction, risk transfer, or risk acceptance.
	5. Regular Risk Review: Risks should be reviewed regularly throughout the project to ensure they are still relevant and to identify new risks.
	6. you should also consider the following factors while identifying and prioritizing risks:
		1. Business Impact: How will the risk affect the business? The higher the potential impact, the higher the risk should be prioritized.
		2. Risk Propagation: How could the risk affect other parts of the project or system?
		3. Risk Appetite: What is the organization's or stakeholder's tolerance for risk? This can affect how risks are prioritized.
		4. Risk Velocity: How quickly could the risk impact the project or system? Faster-moving risks may need to be prioritized higher.
	7. Mitigation and Risk plans:
		1. Risk Management Plan (what can happen with car/driver): This is a broader document that outlines the approach for dealing with risks throughout the project. It includes the methodology, roles and responsibilities, budgeting, timing, risk categories, definitions of risk probability and impact, and the revised stakeholders' tolerances. It also includes the protocols for implementing the risk response, tracking identified risks, and evaluating the effectiveness of the risk response. Risk Management Plan answers the following questions: How will risks be identified? Who is responsible for what? How will risks be assessed and prioritized? How will risk response planning, monitoring, and control be carried out?
		2. Risk Mitigation Plan (what should to do if smth specific happen with car and driver): This is a more specific document that focuses on the strategies and actions to reduce the impact or likelihood of identified risks. It is a part of the overall Risk Management Plan. The Risk Mitigation Plan typically includes the identified risks, their severity, the actions needed to reduce or eliminate the risks, the person responsible for those actions, and the timeline for when these actions need to be completed. Basically, the Risk Mitigation Plan answers: What specific actions will be taken to reduce or eliminate the risks? Who will carry them out? When should these actions be completed?
18. Describe a situation where risk-based testing helped you focus testing efforts on critical areas.

##### Risk Management:
19. What is the difference between risk identification, risk analysis, and risk mitigation in the context of software testing?
20. How do you communicate and manage risks with stakeholders and project teams?
21. Explain the role of risk management in ensuring the quality and success of a software project.

##### General:
22. Describe a challenging testing scenario you faced, and how you approached and resolved it
23. How can AI models be leveraged for test case generation and optimization? What are the potential benefits and limitations of using AI for this purpose?

##### Work Time Organization:
24. How do you prioritize and organize your tasks and responsibilities as a Quality Specialist
25. What strategies or tools do you use to manage your schedule and to-do lists effectively?
26. Describe a time when you had multiple competing deadlines, and how did you handle the situation to ensure all tasks were completed on time?

##### Staying in the Workflow:
27. As a Quality Specialist, you often have to switch between different tasks and contexts. How do you maintain focus and productivity when transitioning between different activities?
28. Describe a situation where you faced a significant challenge or roadblock that threatened to disrupt your workflow. How did you overcome it and maintain productivity?

##### Preventing Exhaustion:
29. Quality Assurance can be a demanding and stressful role. How do you manage stress and prevent burnout or exhaustion?
30. Describe a time when you felt overwhelmed or exhausted due to work demands. How did you recognize the signs, and what steps did you take to address the situation?
31. As a Quality Specialist, you often have to collaborate with cross-functional teams and stakeholders. How do you handle conflicts or differing opinions in a constructive and professional manner?
	1. Open Communication: Encourage open and respectful communication. Allow everyone to express their opinions and ideas.
	2. Active Listening
	3. Empathy: Try to understand the other person's feelings and perspective
	4. Focus on the Issue, Not the Person
	5. Seek Common Ground: Look for areas where everyone agrees. This can help to build a sense of unity and cooperation
	6. Use Objective Criteria
	7. Involve a Neutral Third Party
	8. Provide Training: Consider providing conflict resolution training to your team. This can help to equip them with the skills they need to handle conflicts constructively
32. Adaptability is essential in the fast-paced software development environment. Can you describe a situation where you had to quickly adapt to changing requirements or priorities? How did you handle the change, and what did you learn from the experience?

feedback
___
##### Have to read 
33. Pyramid of testing
34. BDD and TBD / TDD etc. [Business driven testing: как тестировщику решать задачи бизнеса](https://habr.com/ru/companies/skbkontur/articles/832218/)
35. Definition of Done
36. Definition of Ready
37. Use css vs json path (pro / cons)
38. How we can filter data when we use Vividus and get expression from the SQL / API
39. Vividus issue can be fix by create a ticket to github(?) also
40. Vividus for Customer: all positive features (free, open source, reports etc.)
41. Metrics overview
42. Metric for Customer
43. Requirement Analyzes
##### Structure of answer
45. Use structure for answer firstly and describe all on the high level
46. Provide details per request
##### Just re-fresh
47. Mobile testing: features that belong to mobile phone (battery, orientation etc.)
48. Rejected bug ticket: reproducible, add evidence, add details for reproduce
	1. 1. Review the Bug Report: Ensure that the bug report is detailed and clear. It should include steps to reproduce the issue, expected results, actual results, and any relevant screenshots or log files. A well-documented bug report can minimize misunderstandings.
	2. Open Communication: Initiate a conversation with the developer who returned the ticket. It's possible there might be a misunderstanding or miscommunication about the issue. 
	3. Reproduce the Issue.
	4. Understand Their Perspective
	5. Involve Others If Needed
	6. Escalate If Necessary: If you are confident that the issue is a legitimate bug and it's not being addressed, you may need to escalate the issue to higher management or stakeholders
	7. Maintain Professionalism: Throughout the process, maintain a professional and respectful demeanor. Focus on the issue at hand, not on the individuals involved.
49. Watch session

