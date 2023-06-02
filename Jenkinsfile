pipeline {
  agent any
  tools { 
        maven 'maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asecgurubuggyapp -Dsonar.organization=asecgurubuggyapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=d249a0f96dc4ce34956308ed9be23606b901f521'
			}
        } 
  }
}
