pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggy-project_v1 -Dsonar.organization=buggy-project -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=42d9891fb957a000705c47101a965a73847533bb'
			}
        } 
  }
}
