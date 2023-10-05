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
			steps {
				when {
					expression {
						BRANCH_NAME == 'master'
					}
				}
				script {
					echo "Building the application"
				}
			}
		}
		stage('publish')
		{
			steps {
				when {
					expression {
						BRANCH_NAME == 'master'
					}
				}
				script {
					echo "Building the application"
				}
			}
		}
	}
}
