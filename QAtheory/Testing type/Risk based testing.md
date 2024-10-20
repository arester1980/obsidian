Testing purpose is find the most critical issues as soon as possible
We should:
- analyze what areas are risky
* Plan testing them more and early
- Reduce testing effort for other areas

All of our next activity will be based on this work.

Risk attribute
- Impact - cost of bug
- Probability - chance of bug

We should to find balance between these two factors.

Algorithm:
1. Find 10 most important features and evaluate what worth can happen (system down, application crash, how often will use this feature etc)
2. Find the
	* most ambiguous requirements
	* which had a lot of issues in past
	* technological complex
	* logically complex
	* which implement by junior developer
	* which developed in rush
	* which get a lot of changes
___
You can also analyze bug reports from past and find most critical bug in most critical feature for decide which test cases should be run first of all. For example: if in feature "Cart" we have a lot of regression bugs we need to run all test cases, but if we have minor bag in less important feature we can run only smoke test (for save time).  
Also we can base on browser or device usage statistics for prioritize test case.  
Review testing plan and focus activity on every sprint.
___
##### Как бы вы реализовали стратегию тестирования с учетом рисков?
> В стратегии тестирования с учетом рисков первым шагом будет выявление потенциальных рисков в программном обеспечении, которые могут повлиять на его функциональность или производительность. Затем эти риски распределяются по приоритетам в зависимости от их влияния на приложение и вероятности возникновения. Такой подход гарантирует, что наиболее критичные области ПО будут тщательно протестированы.