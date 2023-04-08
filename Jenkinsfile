pipeline {
  agent any
  tools { 
        maven 'Maven_3.5.2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=narutobuggwebapp -Dsonar.organization=narutobuggwebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=d8e2f04664c87c739378fe286ce38ca46b12a2c7'
			}
        } 
  }
}
