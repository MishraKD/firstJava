pipeline {
	     agent any
	     stages{
	     stage('SCM') {
	            steps {
	                git url: 'https://github.com/rohan0903/Devops.git'
	            }
	        }
	    stage('SAST') {
	        steps {
	                withSonarQubeEnv('My SonarQube Server') {
	                   
	                    withMaven(maven:'Maven 3.0.4') {
	                        sh 'mvn clean package sonar:sonar'
	                    }
	                }
	            }
	    }
	     
	     }
	}
