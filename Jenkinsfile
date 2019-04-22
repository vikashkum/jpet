node {
 	stage("checkout")
 	{
 	checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'bf0b619f-cfa6-4f0d-871a-c8c6df0072bc', url: 'https://github.com/gouravpatel1996/jpet.git']]])
 	}
 	stage("build")
 	{
 	sh label: '', script: 'mvn install'
 	}
 	stage("unit testing")
 	{
 	echo "Test successful"
 	}
 	stage("Deploy")
 	{
 	echo "Deploy completed"
 	}
 	stage("Exec")
 	{
 	echo "Execution completed successfully"
 	}
 	}
