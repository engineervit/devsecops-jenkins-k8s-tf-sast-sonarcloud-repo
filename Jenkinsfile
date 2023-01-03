pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp2 -Dsonar.organization=asgbuggywebapp2 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=2ba495e64e5be2e9801e950c45b2f9d522599cba'
			}
        } 
  }
}
