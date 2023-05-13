pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=secureat -Dsonar.organization=secureat -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=96907d895e00d6e86b15659b3f7a3edc73ee68c5'
			}
        } 
  }
}
