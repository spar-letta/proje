pipeline{
	agent any
	
	  stages {
		stage ('Compile Stage'){
		
			steps{
				withMaven(maven : 'maven'){
				sh 'mvn clean compile'				
				}			
			
			}		
		
		}
		stage('Testing Stage'){
		
			steps{
				withMaven(maven : 'maven'){
				sh 'mvn test'				
				}			
			
			}
		
		}
		
		stage('Deloyment Stage'){
		
			steps{
				withMaven(maven : 'maven'){
				sh 'mvn deploy'				
				}			
			
			}
		
		}
	}
	
}
