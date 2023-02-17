pipeline {
  agent any
  tools { 
        maven 'Maven_3.5.2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp12 -Dsonar.organization=asgbuggywebapp12 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=ff1c0730f97d2e70925d6c8e9c5c2307cf0ead34'
			}
        } 
  }
}
