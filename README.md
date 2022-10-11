# README


try

```
./gradlew -q --init-script=./init.d/init.gradle

```

output 


```
During: Init-Phase: root project 'myPublish':[pluginMaven]
[pluginMaven]
After Init-Phase: root project 'myPublish':[myPluginPluginMarkerMaven, pluginMaven]

```

expected output:

Same behavior as gradle < 5.0:  
An array which contains `myPluginPluginMarkerMaven` publication in the init-phase too. 
