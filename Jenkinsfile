pipeline{
	agent any
	
	  stages {
		stage ('Compile Stage'){
		
			steps{
				git url : 'https://github.com/spar-letta/proje'
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
