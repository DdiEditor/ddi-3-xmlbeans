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
1. Modify, the [project_home]/build.properties to point to the directory of the
   ddi3 schemas directory and set the name of the output jar file
2. The project lib-java holding the XmlBeans jars needs to be checked out from 
   version controle as weel at: ../[project_home]
3. Execute in shell at [project_home] ant to run ANT target 'scomp'

// ant properties
See: http://xmlbeans.apache.org/docs/2.0.0/guide/antXmlbean.html for additional 
ANT task scomp settings

// usage
When using the generated classes refer to the generated jar:
[project_home]/xmllib/org.ddialliance.ddi_3_0_xxx.xml.xmlbeans.jar because it 
includes some XmlBean specific filemappings from Java to XML schema. 

