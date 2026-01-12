pipeline {
    agent any

    stages {

        stage('Checkout Code from GitHub') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/GOSHIKASNEHA/Demo.git'
            }
        }

        stage('Install Dependencies') {
            steps {
                sh 'pip install pytest'
            }
        }

        stage('Run Test Cases') {
            steps {
                sh 'pytest'
            }
        }

        stage('Build Success') {
            steps {
                echo '✅ Jenkins Pipeline executed successfully!'
            }
        }
    }
}
