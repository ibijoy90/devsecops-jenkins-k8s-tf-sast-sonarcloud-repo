pipeline {
  agent any
  tools { 
        maven 'Maven_3.8.4'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify org.sonarsource.scanner.maven:sonar-maven-plugin:sonar -Dsonar.projectKey=iphone -Dsonar.organization=iphone -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=34b116ff9535ddaf409e48acc7f1245327112470'
			}
        } 
  }
}
