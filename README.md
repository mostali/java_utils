# java_utils


## Create a template string for class with name 'TestBean' and two fields
```
GenBeanClass gen = GenBeanClass.of("TestBean Long longFiled String stringFiled");
//or new GenBeanClass("TestBean", "Long", "longFiled", "String","stringFiled"); 

gen.generateAndPrint();
```

## Create a template string for class with name 'TestBeanFinal' and two final fields
```
GenBeanClass genf= GenBeanClass.of("final TestBeanFinal Long longFiled String stringFiled");
//or new GenBeanClass("TestBeanFinal", "Long", "longFiled", "String","stringFiled").setIsFinal(true);

genf.generateAndPrint();
```
