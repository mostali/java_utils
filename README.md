# java_utils

     /**
		 * Create a template string for class with name 'TestBean' and two
		 * fields
		 */
		GenBeanClass gen = GenBeanClass.of("TestBean Long longFiled String stringFiled");
		// new GenBeanClass("TestBean", "Long", "longFiled", "String",
		// "stringFiled");
		gen.generateAndPrint();

		/**
		 * Create a template string for class with name 'TestBeanFinal' and two
		 * final fields
		 */
		gen = GenBeanClass.of("final TestBeanFinal Long longFiled String stringFiled");
		// new GenBeanClass("TestBeanFinal", "Long", "longFiled", "String",
		// "stringFiled").setIsFinal(true);
		gen.generateAndPrint();
