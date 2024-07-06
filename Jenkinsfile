pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=easybuggyapp01mk -Dsonar.organization=easybuggyapp01mk -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=f0f336af75a237f0103af1dc4b84c5cdb7c9aeb0'
			}
        } 
  }
}
