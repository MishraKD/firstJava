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
	                
              sh '/var/jenkins_home/yasca/yascaConfigScript/yascaConfigScritp.sh'
	                       
	                    
	                
	            }
	    }
	     
	     }
	}
