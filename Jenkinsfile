pipeline {
	agent any	
	stages {
		            stage('SCM') {
		            steps {
		                git url: 'https://github.com/MishraKD/assin11.git'
		            }
		        }
		
		
		stage('Apply Kubernetes Files') {
      steps {
          withKubeConfig([credentialsId: 'kubeconfig']) {
         sh 'kubectl apply -f deploymentfile.yaml'
        }
      }




   }
}

             


	                       	                
	     



