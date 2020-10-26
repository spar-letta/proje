node {
  stage ('SCM Checkout') {
    git url: 'https://github.com/spar-letta/proje'
  }
    stage ('Compile-Package') {
	    sh 'mvn package'
  }
}
