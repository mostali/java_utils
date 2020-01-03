# java_utils


## Example №1. Create a template string for class with name 'TestBean' and two fields
```
GenBeanClass gen = GenBeanClass.of("TestBean Long longFiled String stringFiled");
//or new GenBeanClass("TestBean", "Long", "longFiled", "String","stringFiled"); 

gen.generateAndPrint();
```
### RESULT
```
public class TestBean {
		private Long longFiled;
		private String stringFiled;

		public TestBean(Long longFiled, String stringFiled) {
			this.longFiled = longFiled;
			this.stringFiled = stringFiled;
		}

		public Long getLongFiled() {
			return this.longFiled;
		}

		public void setLongFiled(Long longFiled) {
			this.longFiled = longFiled;
		}

		public String getStringFiled() {
			return this.stringFiled;
		}

		public void setStringFiled(String stringFiled) {
			this.stringFiled = stringFiled;
		}
	}
```

## Example №2.  Create a template string for class with name 'TestBeanFinal' and two final fields
```
GenBeanClass genf= GenBeanClass.of("final TestBeanFinal Long longFiled String stringFiled");
//or new GenBeanClass("TestBeanFinal", "Long", "longFiled", "String","stringFiled").setIsFinal(true);

genf.generateAndPrint();
```
### RESULT
```
public class TestBean {
		private Long longFiled;
		private String stringFiled;

		public TestBean(Long longFiled, String stringFiled) {
			this.longFiled = longFiled;
			this.stringFiled = stringFiled;
		}

		public Long getLongFiled() {
			return this.longFiled;
		}

		public void setLongFiled(Long longFiled) {
			this.longFiled = longFiled;
		}

		public String getStringFiled() {
			return this.stringFiled;
		}

		public void setStringFiled(String stringFiled) {
			this.stringFiled = stringFiled;
		}
	}
```
```
