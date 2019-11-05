pipeline {
		     agent any
	
		     stages{
		     stage('SCM') {
		            steps {
		                git url: 'https://github.com/MishraKD/assin11.git'
		            }
		        }
			    
		    stage('soapui & regression') {
	        steps {
			
			sh '/var/jenkins_home/soapui/SoapUI-5.2.1/bin/testrunner.sh -s"TestSuite 1" -c"TestCase 1" -r /var/jenkins_home/workspace/deployKubeApp_SoapUi/REST-Project-1-soapui-project.xml'
			
			
			

			//bat 'c:/jmeter/bin/jmeter.bat -n -t c:/jmeter/extras/Test.jmx -l test.jtl'
			//sh '/var/jenkins_home/JMeter/jakarta-jmeter-2.5/bin/jmeter.sh -n -t $WORKSPACE/microservice/performance-scripts/$JMX.jmx -l $WORKSPACE/$JMX.jtl'
	                
             
	                       
	                    
	                
	            }
	    }


		     
		     }
		}
