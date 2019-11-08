pipeline {
	agent any
	
	stages {

             stage('SCM') {
		            steps {
		                git url: 'https://github.com/MishraKD/assin11.git'
		            }
		        }

		
		stage('DeployToProduction') {
             steps {

            
             kubernetesDeploy(

                    kubeconfigId: 'kubeconfig',

                    configs: 'deploymentfile.yml',

                    enableConfigSubstitution: true   
             )

            }
		}



   }
}
