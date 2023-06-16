pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=fsbuggyapp -Dsonar.organization=fsbuggyapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=5c882402f4e2f8f3ee4954a46084cb90548f2bfc'
			}
        } 
  }
}
