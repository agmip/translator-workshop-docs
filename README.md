# AgMIP Translator Sprint #

## Update to latest translator versions (Manually)
* Visit http://github.com/agmip/agmip-core/tags and download the latest zip file.
* Visit http://github.com/agmip/translator-dist/tags and download the latest zip file.
* Uncompress both zip files
* Open both projects in your IDE and initiate ```Maven: Install```
__OR__
* From the command line run: ```mvn install``` in each project directory.
(__NOTE__: agmip-core may say BUILD FAILED due to lack of authentication, this is okay)

## Update the pom.xml file for your translator
You need to update the ```pom.xml``` file for your translator to reflect the
new version of the translator-dist.
```XML
<parent>
    <groupId>org.agmip.translators</groupId>
    <artifactId>translator-dist</artifactId>
    <version>0.6</version>
</parent>
```


## Setup the Github Repository
* From __your__ Github account, click _New Repository_. 
* Name it ```translator-<model>```
* Should be marked as Public
* Click create

## Inform the translator-dist of the new project
* From the AgMIP github page, load up translator-dist
* Click on __Issues__
* Create new issue with the name of your translator
