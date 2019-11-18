pipeline {
	
agent any	
	stages {
		           
				    stage('codeQuality & analysis') {
		        steps {
				git url: 'https://github.com/MishraKD/assin11.git'
				
		                withSonarQubeEnv('sonar') {
					
		                   
		                    withMaven(maven:'M2_HOME') {
					    sh 'mvn clean package sonar:sonar'
		                        
		                    }
		                }
		            }
		       }



         

		          	    




            
stage('DeployToProduction') {
             steps {
		  
            
             kubernetesDeploy(
		     
		    

                    kubeconfigId: 'kubeconfig1',

                    configs: 'deploymentfile.yml',

                    enableConfigSubstitution: true   
             )

            }
		}
		




   }
}

             



             


	                       	                
	     



