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
	                
             
             sh 'jmeter.sh -n -t $WORKSPACE/microservice/performance-scripts/$JMX.jmx -l $WORKSPACE/$JMX.jtl'

	                       
	                    
	                
	            }
	    }
	     
	     }
	}
