pipeline {
		     agent any
		     stages{
		     stage('SCM') {
		            steps {
		                git url: 'https://github.com/MishraKD/assin11.git'
		            }
		        }
		    stage('codeQuality & analysis') {
		        steps {
		                withSonarQubeEnv('sonar') {
		                   
		                    withMaven(maven:'Maven 3.0.4') {
		                        sh 'mvn clean package sonar:sonar'
		                    }
		                }
		            }
		    }
		     
		     }
		}
