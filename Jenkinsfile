pipeline{
	agent any 
	stages{
		stage('1-clonecode'){
			steps{
				checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[credentialsId: 'Team7-git-id', url: 'https://github.com/Owusu-77/Jenkins.git']])
			}
		}
		stage('2-artifactbuild'){
			steps{
				sh 'df -h'
			}
		}
		stage('3-unitest'){
			steps{
				sh 'lscpu'
                                sh 'pwd'
                                sh 'whoami'
			}
		}
		stage('4-deploy'){
			steps{
				echo "We are on pipeline as code module"
			}
		}
			stage('5-Newdeploy'){
			steps{
				echo "This is a final deploy!!"
			}
		}
		stage('6-Security Check'){
			steps{
				sh "bash -x /var/lib/jenkins/workspace/Team7-pipeline-Demo1/pipeline.sh"
			}
		
	}
	
}
}