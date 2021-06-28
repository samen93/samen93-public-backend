pipeline {

    agent {
        node {
			label 'backend'
		}
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh '''
                    echo "Multiline shell steps works too"
                    npm install 
                    npm start
                '''
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