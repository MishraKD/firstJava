pipeline {
	     agent any
	     stages{
	     stage('SCM') {
	            steps {
	                git url: ''
	            }
	        }
	    stage('soapui') {
	        steps {
			
			sh /var/jenkins_home/soapui/SoapUI-5.2.1/bin/testrunner.sh -s"TestSuite 1" 
			-c"TestCase 1" -r /var/jenkins_home/workspace/KuberTesting2_SoapUi/REST-Project-1-soapui-project.xml
	                
             
             

	                       
	                    
	                
	            }
	    }
	     
	     }
	}
