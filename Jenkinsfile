pipeline {
  agent any
  tools { 
        maven 'M2_HOME'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=claudele92_devsecops-pipeline-project -Dsonar.organization=claudele92 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=7c06b0ca05c411c7914ff4152b9cf01858102e57'
			}
        } 
  }
}
