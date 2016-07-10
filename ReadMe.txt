1. cd into E:\pgm\pgm\maven\MyFirstMavenProject directory
2. mvn archetype:generate - create structure for a specific type of project
3. mvn eclipse:eclipse - make a maven project as Eclipse project

In Eclipse:
4. execute a maven project: maven build - will create a run configuration
	a) Create package file- Goals= package
		i) Simple java application: jar file is created
		ii) Java web application: war file is created
	b) Run without integrated server- Goals= tomcat:run
	c) Clean created package- Goals= clean
	d) Clean created package && create new package- Goals= clean package
	e) Create runnable jar file- Goals= clean package assembly:single
5. To auto completion of dependency in pom file,
show view -> other -> Maven -> Maven Repositories ->
Local Repositories -> Local Repository -> Right click ->
Rebuild Index

6. Add Archetype Catalog
Go to menu Window--->Preferences.
At the Preferences window, select Maven---->Archetypes,
On the Right Panel, click Add Remote Catalog... button.
At the Remote Archetype Catalog windows enter the following: -
Catalog file: http://repo.maven.apache.org/maven2
Description: Maven Central