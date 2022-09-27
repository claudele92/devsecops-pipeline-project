pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggyapp-pipeline -Dsonar.organization=buggyapp-pipeline -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=fa6c222b458e33a3c2fe60bc72ea74e534b4538a'
			}
        } 
  }
}
