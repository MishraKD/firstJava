pipeline {
	     agent any
	     stages{
	     stage('SCM') {
	            steps {
	                git url: 'https://github.com/MishraKD/assin11.git'
	            }
	        }
	    stage('SAST') {
	        steps {
	                
             sh '/var/jenkins_home/JMeter/jakarta-jmeter-2.5/bin'
             sh 'jmeter.sh -n -t $WORKSPACE/microservice/performance-scripts/$JMX.jmx -l $WORKSPACE/$JMX.jtl'

	                       
	                    
	                
	            }
	    }
	     
	     }
	}
