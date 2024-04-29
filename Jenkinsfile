pipeline {
    agent {
        docker { image 'node' }
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
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
