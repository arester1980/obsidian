1. First we should download and unzip **MAESTRO-CLI**
2. Run **windows-console.cmd**
3. Go to cloud.epam and pass **\"ACTIVATE PROJECT"**
4. run in CLI[^1] _or2-get-access_ > copy url and go > copy and insert access code to CLI
	* id and token should be response
5. Checking available regions, images and shapes
	* **or2-describe-regions -p personal[^2] -t EPAM[^3]**
	* **or2-describe- #images -p personal -r epam-by2[^4]** ^72e947
	* **or2-describe- #shapes -p personal -r epam-by2** ^37faee
6. for create run **or2run -p personal -r epam-by2 -i [[#^72e947|Win10-64]] -s [[#^37faee|medium]]**

### INSTANCE = IMAGE(_OS+HDD_) + SHAPE FLAVOR(_CPU + RAM_) + [ VOLUME(_if necessary_) ]

[^1]: be sure that vpn is used
[^2]: -p mean names of project
[^3]: -t EPAM, AWS, GOOGLE
[^4]: -r means region