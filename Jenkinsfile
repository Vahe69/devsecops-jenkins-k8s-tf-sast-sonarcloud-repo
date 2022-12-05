pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebappjenkins -Dsonar.organization=asgbuggywebappjenkins -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=50ba351e7e4791719fcc0ffb5264f74937e328ac'
			}
        } 
  }
}
