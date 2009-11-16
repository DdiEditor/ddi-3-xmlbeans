// outline
The project uses an ANT build file
Buildfile: build.xml

Main targets:

 clean    Clean project
 init     Set up project
 javadoc  Compile javadoc for compiled schema code
 scomp    Compiles a schema into XML Bean classes and metadata
Default target: scomp

// build project
1. The project 'lib-java' holding the XmlBeans jars needs to be checked out from source 
   version control as weel at: ../[project_home]
2. The project needs internet access to checkout the DDI schemas from the DDI source 
   version control at SourgeForge
2a.Waiting DDI-TIC to put ddi-3.1 into the repository at sf.net Until then download the 
	ddi-3.1 schema file into the location defined in build.properties waiting.tic.fix.localcopy.schema.dir         
3. Execute in shell at [project_home] ant to run ANT target 'scomp'

// ant properties
See: http://xmlbeans.apache.org/docs/2.0.0/guide/antXmlbean.html for additional 
ANT task scomp settings

// usage
When using the generated classes refer to the generated jar:
[project_home]/xmllib/org.ddialliance.ddi3.xml.xmlbeans.jar because it 
includes some XmlBean specific filemappings from Java to XML schema. 

