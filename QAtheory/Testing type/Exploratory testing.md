**Exploratoty** is a kind of testing. It means that we should have all documentation from requirements to reports.
**Ad Hoc** is a part of Exploratory. There isn't any docs. We should just work with application.

#### Basic Style
- Questioning
- Similarity to previous (**read forum!**)
- Gossip and Prediction (be careful and listen to team member)
- Improvisation
#### Model Style
- Architecture
- Bubble (scheme and graph)
- Data relationship
#### Examples Style
- [BDD](joplin://2ac93c8dfca84b029e977877e1c06ee7)
- Positive testing
- Simple walkthrough
- Soap operas (it's a variant of User Story but with ENORMOUS and STRANGE details)
#### Invariance Style
- small changes in input data
#### Interference Style
- Interrupt / Stop / Pause
- Compete (different action at the same time)
#### Error Handling Style
- work with error which expected (raise error many time a row for exmpl)
#### Group insight Style
- Brainstorm
- Fishbone analysis
#### Districts & Tours

---

**Business** - A business district is a place where people make money. Here you can find a lot of banks and office buildings. In several cases, tourists do not like to walk in the business district as there is nothing interesting to see.|Some tourists travel only according to the guidebook and never visit places that are not included or mentioned in the guide. This situation is relevant to the users who strictly follow each and every step specified in the support information, instructions, and user manuals. A software product also has its own “business district” features that are designed to increase sales. Promo material informs about the features that differentiate a software product from similar ones available on the market and attract more users. For Example, a free trial period, every 5th delivery is free, etc.

| Guidebook                                                                                                                                                                                                                                                                          | Money                                                                                                                                                                                                                                                           | Landmark                                                                                                                                                                                                                              | Intellectual                                                                                                                                                                                                          | FedEx                                                                                                                                                                                                                                                                                 | After-Hours                                                                                                                                                                                   | Garbage-Collector                                                                                                                                      |
| ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Some tourists travel only according to the guidebook and never visit places that are not included or mentioned in the guide. This situation is relevant to the users who strictly follow each and every step specified in the support information, instructions, and user manuals. | Every city has a special place that attracts all the tourists. For Example, people visit Paris to see the Eiffel Tower and the Louvre museum. The visiting card of Rome is the Colosseum.                                                                       | A tourist selects the places to visit beforehand but without detailed planning as he/she does with a guidebook. A test engineer defines a list of software features and executes testing based on that list in a step-by-step manner. | Every tourist group will include a person who would have read tons of books about the city, its history, cultural traditions and try to show his/ her brilliance all the time.                                        | Before reaching an addressee, an international parcel gets additional marks and ticks.                                                                                                                                                                                                | At the end of the working day, people go home leaving their job for the next day. But when a user closes an application, that does not mean that it stops working totally.                    | Even the smallest town has garbage collectors who spend a couple of minutes near every house to collect garbage and go farther.                        |
| Users may face such bugs as unclear/improper instructions, steps to follow do not correspond the actual work of software, inconclusive prompts, etc.                                                                                                                               | In software testing, the advertising materials should correspond to the actual features of the application. Otherwise, after purchasing the application, the users will be disappointed, might leave negative feedback, and never recommend your app to others. | Thus, the tester does not miss the critical functionality and may detect bugs that block the system’s operability.                                                                                                                    | A tester also can execute untypical user scenarios to detect bugs. For Example, to enter a very long name for a file, add a huge number of products to the shopping cart, enter invalid data to the form fields, etc. | A software product also utilizes data that can be stored, modified, or even lost. A test engineer should follow the way in which the data is processed and validate it after all the operations. For Example, an app does not support the Cyrillic alphabet or right-to-left writing. | The application can backup or archive data, receive updates, etc. Verifying the application in the background mode, a tester can detect irrational usage of traffic, memory leaks, and so on. | In software testing, the tour resembles sampling verification without any detailed analysis. For Example, checking software UI, content elements, etc. |
|                                                                                                                                                                                                                                                                                    | Also, the Money tour may detect outdated screenshots or lists of features, improper grammar, and logical mistakes.                                                                                                                                              |                                                                                                                                                                                                                                       |                                                                                                                                                                                                                       |                                                                                                                                                                                                                                                                                       |                                                                                                                                                                                               |                                                                                                                                                        |

---

**Historic** - A typical tour includes a tour around old districts which is full of ancient buildings and places of historical value. In testing, a historic district means the features connected with the previous product versions, code, or functionality.

|Bad-Neighborhood|Museum|Prior Version|
|---|---|---|
|There are places that tourists should better try to avoid.|Every traditional tour includes visiting museums.|The restoration of buildings is similar to software updates. Users should easily adapt to the updated UI and functionality that can change the user experience.|
|A bad-neighborhood tour is code fragments that contain a lot of bugs. Usually, one bug triggers another one, and so on. A tester should check such buggy areas precisely.|In testing, a museum is a code that developers have not changed for a long time. The code may not work in a new environment. For Example, an Android version of the application operates properly. Developers may copy code or files that are improper for an iOS version.|A tester should take all the modifications into account.|

---

**Entertainment** - After a long walk, the tourists wish to have some fun. An entertainment district symbolizes the option of software customization. Entertainment districts focus on the functionality related to the core one. The tours can help to detect UI bugs, localization errors, usability issues, and uncritical functional bugs.

|Supporting Actor|Back Alley|All-Nighter or Clubbing|
|---|---|---|
|focus no on a critical functionality|testing of not frequently used features|testing an application without restarting|

---

**Tourist** - Every city and town has places where tourists spend a lot of money. Here there are many restaurants and gift shops.  
In testing, a Tourist district means to look through the software functionality without focusing on any detail. A tester may follow the Collector tour and verify software artifacts, E.g., everything that a user is able to save. Also, there are Lonely Businessman (to get to the feature using the longest way), Supermodel (GUI verification), and Scottish Pub tour that includes the analysis of users’ feedback.

|Collector|Lonely Businessman|Supermodel|Scottish Pub|
|---|---|---|---|
|verify software artifacts, E.g., everything that a user is able to save|to get to the feature using the longest way|GUI verification|that includes the analysis of users’ feedback|

---

**Hotel** - Usually, tourists stay in hotels where they can take some rest and relax after a busy day. In testing, a Hotel district is a place to verify the non-critical functionality.

|Rained-Out|Couch Potato|
|---|---|
|Sudden rain can spoil the planned promenade and make tourists stay in the hotel. A tester verifies the system behavior by canceling the previous operation and checks the after-effects of his actions.|A tourist group may include an apathetic person who is not interested in anything.|
||In testing, a QA specialist should verify the system functionality by following a default way without making any settings.|

---

**Seedy** - A seedy district is too dangerous for tourists. In testing, it is such software areas that attract shifty users who strive to crash the system.

|Saboteur|Obsessive-Compulsive|Antisocial|
|---|---|---|
|try to crash the system by limiting the resources that are required for proper operation|repeating the same action several times and monitoring the system behavior|to perform the actions that contradict the app logic, for example, entering invalid data|
|||Opposite - testers perform the actions that the users will conduct unlikely, for example, adding more than 10 000 tracks to a playlist|
|||Crime Spree - to enter illegal data, E.g., SQL injections|
|||Wrong Turn - performs an ordinary action but in the wrong sequence|

[Exaples on Russian](https://software-testing.ru/library/testing/testing-for-beginners/2965-exploratory-software-testing "https://software-testing.ru/library/testing/testing-for-beginners/2965-exploratory-software-testing")