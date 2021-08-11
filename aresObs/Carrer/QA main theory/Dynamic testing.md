__Source:__ [Quality Managment System](htps://epam.sharepoint.com/sites/policy/EPAM%20Regulations/Forms/EPAM%20Regulations.aspx?id=%2Fsites%2Fpolicy%2FEPAM%20Regulations%2FProcess%20Descriptions%2FEPAM%5FDynamicTestingPD%2Epdf&parent=%2Fsites%2Fpolicy%2FEPAM%20Regulations%2FProcess%20Descriptions)

Если совсем кратко, то динамическое тесирование это любое тестирование, связанное с выполнением кода тестируемой программы.

Состоит из 3 активностей:
1. Test Design
	1. создание тест кейсов на основе требований (тест-матрица, тест-кейсы, [[Gherkin]], автоматизация)
1. Test environment setup
	1. настройка тестовой среды
	2. подготовка тестовых данных
	3. установка иснтрументов тестирования
1. Test execution
	1. Execute test-case
	2. recording test results
	3. reporting and analyzing defects

Если проект полностью построен на [[BDD]] то тестовая докуентация является частью _single source of truth_ - единого документа для owner, BA, QA и Dev

**Testing Team Lead[^1] in charge on**

|Focus Area of Manual Testing|Focus Area of Manual Testing|
|---|---|
|определение требований к инфраструктуре, запрос на инфрастуктуру, проверка, что устанволенно все необходимое|определение требований к инфраструктуре, запрос на инфрастуктуру, проверка, что устанволенно все необходимое||
|определение области тестирования, разбиение ее на структуры, выбор наиболее эффективных техник|определение области тестирования, где целесообразно использовать автоматизацию, определение наиболее эффективных техник|
|Измерения, мониторинг и подготовка отчетов отходе тестирования и выявленных багах|Измерения, мониторинг и подготовка отчетов отходе тестирования и выявленных багах|
|Подготовка обзоров|Подготовка обзоров|	

**Key Tester[^2] in charge on**

|Focus Area of Manual Testing|Focus Area of Manual Testing|
|---|---|
|разработка тест кейсов|разработка, внедрение и поддержка тестовых фреймворков|
|ревью тест-кейсов других тестировщиков|разработка и поддержка тест-кейсов|
|Установка и настройка тестового окружения|установка и настройка тестовых окружений или устройств|
|Тестирование|тестирование|
|Анализ результатов тестирования|исправление ошибок в коде, исправления кода в соотвествии с практиками|
|Подготовка отчетов|код ревью|
||рефакторинг кода|
||анализ результатов|
||подготовка отчетов|

**Tester in charge on**

|Focus Area of Manual Testing|Focus Area of Manual Testing|
|---|---|
|разработка тест кейсов|разработка новых и поддержка существующих тест-кейсов|
|выполнение тест-кейсов||
|первоначальный анализ багов|исправление ошибок и рефакторинг|
|информировании команду о критических багах|первоначальный анализ багов|
|контроль исправления багов|настройка окружения и траблшутинг|
|Подготовка отчетов|код ревью|
||подготовка отчетов|

**Inputs and Entry Criteria**

-tx-
|Inputs|Entry|
|:---:|---|
|_For test Design activity_||
|Requirements documentation is available|Project is initiate|
|Test Strategy|DM or PM selects process of testing and Quality Control|
|Available design document|Test Plan is approved and according in can testing activity can starts|
|_Test-Environment set-up activity_ ||
|Test Plan| - |
|Request for Purchase| - |
|_Test execution activity_| - |
|Test cases, Test matrix, Checklist| - |
|Ready data and Environment| - |

** \* - Test data shall not be from prod. Customer should guaranteed that data isn't from prod **

### Process of Manual Test Design ###
1. Read requirements - For __what__ we should testing
2. Read Test Plan / Test Strategy - For __how__ we should testing
3. Base on 1 and 2 prepare the logical document (with user stories, perhaps) and selected form of testing documentation (Checklist, Test-Matrix, Test-Case, priority of features etc.) and Question List
4. Base on 3 writes test-cases
5. Review Test-Cases
6. On approved test-cases executed it.

![Automation](d:/ObsVault/aresObs/Carrer/.pic/Untitled1.png)
![Manual](d:/ObsVault/aresObs/Carrer/.pic/Untitled.png)
![Test Env Set-Up](d:/ObsVault/aresObs/Carrer/.pic/test_env.png)
![Manual Test Execution](d:/ObsVault/aresObs/Carrer/.pic/manual_test_exec.png)
![Automate Test Execution](d:/ObsVault/aresObs/Carrer/.pic/autom_exec.png)

**Outputs and Exit Criteria**

-tx-
|Outputs|Exit|
|:---:|---|
|_For test Design activity_||
|Automated tests|Planned testing has been complete|
|Test Cases| - |
|_Test-Environment set-up activity_ ||
|Configured Test environment and access| - |
|_Test execution activity_| - |
|Test results| TM or PM or DM have signed off and approved of the exec results |
|Defects| Test defects are submitted to BTS |

### Verification criteria ###
* Test cases are reviewed and accepted
* Test environment is verified and accepted
* All results (pass and fail) record and submitted in BTS


_Short article on Russian_: [Статическое и динамическое тестирование](https://testmatick.com/ru/staticheskoe-i-dinamicheskoe-testirovanie/)

[^1]: Level from 3 to 5 or M1 with skills: Functional Testing, Automated Testing, Performance testing, BI Testing or Data Quality
[^2]: High quality Tester