pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecuritygurulbuggywebapp -Dsonar.organization=asecuritygurulbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=6e9d012fba633125448881a21d484f8ccde120d3'
			}
        } 
  }
}
