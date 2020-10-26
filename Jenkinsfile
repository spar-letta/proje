node {
  stage ('SCM Checkout') {
    git url: 'https://github.com/spar-letta/proje'
  }
    stage ('Compile-Package') {
	    def mvnHome = tool name: 'maven', type: 'maven'
	    sh "${mvnHome}/bin/mvn package"
  }
}
