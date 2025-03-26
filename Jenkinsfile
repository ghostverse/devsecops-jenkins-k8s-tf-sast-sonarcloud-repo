pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=Your_project_key -Dsonar.organization=Your_organization_name -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=Your_token_data'
			}
        } 
  }
}
