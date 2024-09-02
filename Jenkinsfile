pipeline {
	agent any
	stages {
	     stage("pulling the code from scm") {
	          steps {
		  	git branch: 'main', url: 'https://github.com/sanjayjangir1093/pipeline2.git'
		  }
	     }
	     stage("build the code") {
	     	  steps {
		  	sh "mvn compile"
			sh "mvn clean package"
		  }
	     }
	}	
}
