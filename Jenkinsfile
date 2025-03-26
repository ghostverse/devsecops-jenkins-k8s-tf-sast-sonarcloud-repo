pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=Ghosty_Devsecops_Test -Dsonar.organization=ghosty-devsecops -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=2bb182612e6aec05ecb6893684c2176ae68e0fbb'
			}
        } 
  }
}
