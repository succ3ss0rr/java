pipeline {
	agent none
	stages {
		stage('test')
		{
			steps{ 
				script{
					echo "Testing the application"
					echo "Executing pipeline for $BRANCH_NAME"
				}
			}
		}
		stage('build')
		{
			when {
				expression {
					BRANCH_NAME == 'master'
				}
			}
			steps {
				script {
					echo "Building the application"
				}
			}
		}
		stage('publish')
		{
			when {
				expression {
					BRANCH_NAME == 'master'
				}
			}
			steps {
				script {
					echo "Building the application"
				}
			}
		}
	}
}
