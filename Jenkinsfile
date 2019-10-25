pipeline {
	     agent any
	     stages{
	     stage('SCM') {
	            steps {
	                git url: 'https://github.com/MishraKD/assin11.git'
	            }
	        }
	    stage('soapui') {
	        steps {
			
			SoapUIPro ( pathToTestrunner: '<path>', pathToProjectFile: '<path>', 
				   testSuite: '[<testSuiteName>]', testCase: '[<testCaseName>]', projectPassword: '[<password>]',
				   environment: '[<environmentName>]' )
	                
             
             

	                       
	                    
	                
	            }
	    }
	     
	     }
	}
