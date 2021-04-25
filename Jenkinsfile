node{
	stage('SCM Checkout'){
		git 'https://github.com/mahesh1b/jenkins'
	}
	stage('Compile-Package'){
		def mvnhm = tool name: 'maven-3', type: 'maven'
		sh "${mvnhm}/bin/mvn package"
	}

}
