pipeline {
  agent any
  tools { 
        maven 'Maven_3-5-2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebappjenkins -Dsonar.organization=asgbuggywebappjenkins -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=e0c8284b8d35aab8fe8a274c81f745302798cfd1'
			}
        } 
  }
}
