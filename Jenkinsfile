pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=FSbuggy2 -Dsonar.organization=FSbuggy2 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=08810a26ecd1081ee8b1f111d9751036298ba0fa'
			}
        } 
  }
}
