pipeline {
    agent {
        docker {
            image 'node'
            label 'agent-template'
        }
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
		 echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
		sh 'node --version'
                sh 'npm --version'
		sh 'npm run build'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
