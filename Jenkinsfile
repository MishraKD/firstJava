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
	                
             PERFORMANCE_PATH ="/var/jenkins_home/JMeter/jakarta-jmeter-2.5/bin"
               cd '$PERFORMANCE_PATH'
               sh 'jmeter.sh -n -t $WORKSPACE/microservice/performance-scripts/$JMX.jmx -l $WORKSPACE/$JMX.jtl'

	                       
	                    
	                
	            }
	    }
	     
	     }
	}
