node{
	stage('SCM Checkout'){
		git 'https://github.com/mahesh1b/jenkins'
	}
	stage('Compile-Package'){
		def mvnhm = tool name: 'maven-3', type: 'maven'
		sh "${mvnhm}/bin/mvn package"
	}
	stage('Email Notification'){
	mail bcc: '', body: 'Completed successfully.', cc: '', from: '', replyTo: '', subject: 'Jenkins pipeline', to: 'mahesh22071999@gmail.com'
	}

}
