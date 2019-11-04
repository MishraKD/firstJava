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
					sh 'mvn clean package sonar:sonar'
		                   
		                   // withMaven(maven:'Maven 3.6.2') {
		                        
		                   // }
		                }
		            }
		    }
		     
		     }
		}
