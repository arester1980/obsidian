| Smoke Testing                                                                                                           | Sanity Testing                                                                                                           |
| ----------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------ |
| Smoke Testing is performed to ascertain that the critical functionalities of the program is working fine                | Sanity Testing is done to check the new functionality/bugs have been fixed                                               |
| The objective of this testing is to verify the “stability” of the system in order to proceed with more rigorous testing | The objective of the testing is to verify the “rationality” of the system in order to proceed with more rigorous testing |
| This testing is performed by the developers or testers                                                                  | Sanity testing in software testing is usually performed by testers                                                       |
| Smoke testing is usually documented or scripted                                                                         | Sanity testing is usually not documented and is unscripted                                                               |
| Smoke testing is a subset of Acceptance testing                                                                         | Sanity testing is a subset of Regression Testing                                                                         |
| Smoke testing exercises the entire system from end to end                                                               | Sanity testing exercises only the particular component of the entire system                                              |
| Smoke testing is like General Health Check Up                                                                           | Sanity Testing is like specialized health check up                                                                       |
- Both Sanity and Smoke testing are ways to avoid wasting time and effort by quickly determining whether an application is too flawed to merit any rigorous testing.
- Smoke Testing is also called tester acceptance testing.
- Smoke testing performed on a particular build is also known as a build verification test.
- One of the best industry practice in software engineering, is to conduct a Daily build and smoke test in software projects.
- Both smoke and sanity tests can be executed manually or using an automation tool. When automated tools are used, the tests are often initiated by the same process that generates the build itself.
- As per the needs of testing, you may have to execute both Sanity and Smoke Tests in the software build. In such cases, you will first execute Smoke tests and then go ahead with Sanity Testing.
- In industry, test cases for Sanity Testing are commonly combined with that for smoke tests, to speed up test execution. Hence, it’s a common that the terms are often confused and used interchangeably
___
### Advantages of sanity testing

- **Speed**: Sanity testing does not necessitate documentation, enabling quick identification of defects or assurance of their absence. This agility is particularly beneficial when testing time is limited, providing prompt feedback to swiftly address critical issues.
- **Efficiency**: It serves as an effective means to verify that minor changes or modifications to the system have not induced unforeseen side effects or disruptions to existing functionality.
- **Focus**: Sanity testing enables testers to concentrate on specific areas of the system, ensuring that alterations made therein do not result in unexpected consequences.
- **Cost-effectiveness**: Generally, sanity testing requires minimal resources and time for completion. Detecting software issues during sanity testing leads to the rejection of defective builds, saving time and effort that would otherwise be spent on regression testing. Moreover, it aids in identifying significant issues early in the development cycle, thereby averting costly rework in later stages.
- **Increased productivity**: By allowing developers and testers to focus on more complex test scenarios, sanity testing enhances overall productivity and reduces the time needed for full regression testing.

### Disadvantages of sanity testing

- **Limited scope**: Sanity testing focuses on a subset of functional capabilities of the application, potentially overlooking issues or errors outside its scope.
- **Incomplete testing**: It provides only a preliminary assessment of the software's performance and quality, failing to offer a comprehensive view of its functionality.
- **Possibility of false positives**: Due to its rapid nature, sanity testing may yield results indicating proper functionality when defects or issues exist undetected.
- **Dependence on experience**: The effectiveness of sanity testing relies heavily on the experience and expertise of the tester, necessitating a profound understanding of the software's critical functions for accurate testing.