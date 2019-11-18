pipeline {
	
agent any	
	stages {
		           
				    stage('codeQuality & analysis') {
		        steps {
				
		                withSonarQubeEnv('sonar') {
					
		                   
		                    withMaven(maven:'M2_HOME') {
					    sh 'mvn clean package sonar:sonar'
		                        
		                    }
		                }
		            }
		       }
                        		    stage('SAST') {
	        steps {
	                
              sh '/var/jenkins_home/yasca/yascaConfigScript/yascaConfigScritp.sh'
	                       
	                    
	                
	            }
	    }




         

		          	    




            
stage('DeployToProduction') {
             steps {
		  git url: 'https://github.com/MishraKD/assin11.git'
            
             kubernetesDeploy(
		     
		    

                    kubeconfigId: 'kubeconfig1',

                    configs: 'deploymentfile.yml',

                    enableConfigSubstitution: true   
             )

            }
		}
		




   }
}

             



             


	                       	                
	     



