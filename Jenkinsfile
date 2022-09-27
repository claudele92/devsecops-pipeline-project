pipeline {
  agent any
  tools { 
        maven 'M2_HOME'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=claudele92_devsecops-pipeline-project -Dsonar.organization=claudele92 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=589b4eba20c7a261ad7b9a418f6f7698985945b2 -Dsonar.sources=src -Dsonar.java.binaries=.'
			}
        } 
  }
}
