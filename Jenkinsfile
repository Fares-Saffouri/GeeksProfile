pipeline{

	agent any

	environment {
		DOCKERHUB_CREDENTIALS=credentials('dockerhub-fares')
	}

	stages {

		stage('Build') {

			steps {
				sh 'sudo docker build -t fares111/geeksprofile:geeksprofile .'
			}
		}

		stage('Login') {

			steps {
				sh 'sudo echo $DOCKERHUB_CREDENTIALS_PSW | sudo docker login -u $DOCKERHUB_CREDENTIALS_USR --password-stdin'
			}
		}

		stage('Push') {

			steps {
				sh 'sudo docker push fares111/geeksprofile:geeksprofile'
			}
		}
	}

	post {
		always {
			sh 'sudo docker logout'
		}
	}

}
