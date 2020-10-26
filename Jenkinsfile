pipeline{
	agent any
	
	 stages {
		stage ('Compile Stage'){
		
			     git url :'https://github.com/spar-letta/proje'	
				withMaven(maven : 'maven'){
				sh 'mvn clean compile'				
				}			
			
					
		
		}
		
		
		
	}
	
}
