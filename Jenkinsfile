pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=fsbuggyapp -Dsonar.organization=fsbuggyapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=aeae04c2f79dcef48da982f53fd7f98602234a8e'
			}
        } 
  }
}
