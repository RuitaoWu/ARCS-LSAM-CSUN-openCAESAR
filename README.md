# ARCS-LSAM-CSUN-openCAESAR  
## Implementing [openCAESAR](https://github.com/opencaesar) to create an ontology  
```
git clone  https://github.com/RuitaoWu/ARCS-LSAM-CSUN-openCAESAR.git  
cd ARCS-LSAM-CSUN-openCAESAR
gradle build  
``` 
- Encouter the following error:  
```  
* Where:
Build file 'C:\Users\ruita\Desktop\ARCS-LSAM-CSUN-openCAESAR\build.gradle'

* What went wrong:
Could not compile build file 'C:\Users\ruita\Desktop\ARCS-LSAM-CSUN-openCAESAR\build.gradle'.
> startup failed:
  General error during semantic analysis: Unsupported class file major version 61

  java.lang.IllegalArgumentException: Unsupported class file major version 61
```  
- Solution:  
Find proper gradle version [Gradle Compatibility Matrix](https://docs.gradle.org/current/userguide/compatibility.html#java)  
```  
I have java version '17.0.0.1'
change the following line in "gradle.properties" file, and comment the original one:  
which was distributionUrl=https\://services.gradle.org/distributions/gradle-6.5.1-bin.zip  
distributionUrl=https\://services.gradle.org/distributions/gradle-7.3.3-bin.zip  

```  
### The Flowchart that used to create an ontology (Fixed the low pixel issue)  
![Flowchart](https://github.com/RuitaoWu/ARCS-LSAM-CSUN-openCAESAR/blob/main/image/uml.jpg)  