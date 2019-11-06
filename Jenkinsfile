pipeline {
	agent any
	
	stages {

        stage('code-quality') {

            when {

                branch 'master'

            }

            steps {

                script {

                                   withSonarQubeEnv('sonar') {
					
		                   
		                    withMaven(maven:'M2_HOME') {
					    sh 'mvn clean package sonar:sonar'
		                        
		                    }
		                }

                    

                }

            }

        }

    }
}
