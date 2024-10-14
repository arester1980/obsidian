1. Allure display issue
	- `about:config`
	- `privacy.file_unique_origin` to `false`
	- security.fileuri.strict_origin_policy = false

## Technical Know-issues

| #   | Description                                                                                                                                                     | Solution       |
| --- | --------------------------------------------------------------------------------------------------------------------------------------------------------------- | -------------- |
| 1   | Error: Could not find or load main class org.gradle.wrapper.GradleWrapperMain Caused by: java.lang.ClassNotFoundException: org.gradle.wrapper.GradleWrapperMain | gradle -v      |
|     |                                                                                                                                                                 | gradle wrapper |
| 2   | could not found in VC                                                                                                                                           | ./gradlew cE e |
#### jBehave
sintaxis of story doesn't recognize
* right click on the any story
* open with...
* select jbehave
* checkbox 'apply to all '* . story' files
* ok