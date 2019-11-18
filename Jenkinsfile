pipeline {
	
agent any	
	stages {



            
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

             



             


	                       	                
	     



