pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecopsbuggywebapp916 -Dsonar.organization=devsecopsbuggywebapp916 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=62b78e4b469896b247059d5940b3985d2ae293fc'
			}
        } 
  }
}
