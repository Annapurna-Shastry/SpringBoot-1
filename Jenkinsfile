import jenkins.model.*
jenkins = Jenkins.instance
node{
	def mvnHome=tool name: 'Maven', type: 'maven'
		stage('---CLEAN--'){
			echo "clean TEst"
			git config --global --unset-all remote.origin.proxy
			git 'https://github.com/thogeti/SpringBoot.git'
			echo ${mvnHome}
			sh '${mvnHome}/bin/mvn clean package'
		//	sh "mvn clean"
			
		}
		stage('---Packeage--'){	
			echo " Pack TEst"
			//def mvnHome=tool name: 'Maven', type: 'maven'
		//	echo ${mvnHome}
			//sh '${mvnHome}/bin/mvn package'
			
		}
	
	
}
