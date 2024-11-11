pipeline {
    agent any

    stages {
        stage('Clone Repository') {
            steps {
                // Checkout the latest code from GitHub
                git url: 'https://github.com/rajesh-eegala-inn/Python-Pipeline.git', branch: 'main'
            }
        }

        stage('Install Dependencies') {
            steps {
                // Install dependencies for the Python app
                sh 'python3 -m venv venv'
            }
        }



        stage('Run Application') {
            steps {
                // Run the Python application
                echo 'Starting the application...'
                sh './venv/bin/python main.py'
            }
        }
    }
}

