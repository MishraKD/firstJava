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
			//bat 'c:/jmeter/bin/jmeter.bat -n -t c:/jmeter/extras/Test.jmx -l test.jtl'
			sh '/var/jenkins_home/JMeter/jakarta-jmeter-2.5/bin/jmeter.sh'
	                
             // PERFORMANCE_PATH="/var/jenkins_home/JMeter/jakarta-jmeter-2.5/bin"
		//microservice/performance-scripts	
            //cd '$PERFORMANCE_PATH'
			
                             // sh 'jmeter.sh -n -t $WORKSPACE/microservice/performance-scripts/$JMX.jmx -l $WORKSPACE/$JMX.jtl'
	                       
	                    
	                
	            }
	    }


		     
		     }
		}
