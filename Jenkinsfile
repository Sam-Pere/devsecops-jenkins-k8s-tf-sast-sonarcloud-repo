pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=cloud-123 -Dsonar.organization=cloud-123 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=f63c858178d70c73b79c3515f0a4721116b0120f'
			}
        } 
  }
}
