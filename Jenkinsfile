pipeline{
	agent any
	stages{
		stage(1-Clonecodes){
			steps{
			checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'Team7_master_gitid', url: 'https://github.com/Owusu-77/Jenkins.git']])
			}
		}
		stage(2-Build Artifact){
			steps{
				sh 'action2'
			}
		}
		stage(3-Run Test){
			steps{
				sh 'action3'
			}
		}
	}	
}
