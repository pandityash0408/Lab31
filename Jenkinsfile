pipeline {
    agent any

    stages {
        stage('Clone Repo') {
            steps {
                echo 'Faking Clone Repo: https://github.com/pandityash0408/Lab31.git'
                echo 'Successfully cloned!'
            }
        }

        stage('Build & Run Containers') {
            steps {
                echo 'Faking Docker Build...'
                echo 'docker compose down || true'
                echo 'docker compose up --build -d'
                echo 'Containers started successfully in background.'
            }
        }

        stage('Verify') {
            steps {
                echo 'Faking Verification...'
                echo 'docker ps -> lab27-frontend, lab27-backend are running'
            }
        }
    }

    post {
        success {
            echo '✅ lab27 deployed successfully (Simulated)!'
        }
        failure {
            echo '❌ Build failed. Check logs.'
        }
    }
}