pipeline {
		     agent any
		     stages{
		     stage('SCM') {
		            steps {
		                git url: 'https://github.com/MishraKD/assin11.git'
		            }
		        }
		    stage('performance Testing') {
	        steps {
			//sh '/var/jenkins_home/JMeter/jakarta-jmeter-2.5/bin/microservice/performance-scripts'
	                
             // PERFORMANCE_PATH="/var/jenkins_home/JMeter/jakarta-jmeter-2.5/bin"
			
            //cd '$PERFORMANCE_PATH'
               sh 'jmeter -Jjmeter.save.saveservice.output_format=xml -n -t $WORKSPACE/microservice/performance-scripts/$JMX.jmx -l $WORKSPACE/$JMX.jtl'
	                       
	                    
	                
	            }
	    }


		     
		     }
		}
