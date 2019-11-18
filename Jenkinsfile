pipeline {
	
agent any	
	stages {
		
		            stage('SCM') {
		            steps {
		                git url: 'https://github.com/MishraKD/assin11.git'
		            }
		        }

				    stage('codeQuality & analysis') {
		        steps {
				
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

             



             


	                       	                
	     



