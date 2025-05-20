pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Stage 1 -- Build -- Tool: Maven -- running'
                echo 'Stage 1 -- Build -- Tool: Maven -- pass'
            }
        }

        stage('Unit and Integration Tests') {
            steps {
                echo 'Stage 2 -- Unit and Integration Tests -- Tools: JUnit  -- running'
                echo 'Stage 2 -- Unit and Integration Tests -- Tools: JUnit  -- pass'
            }
        }

        stage('Code Analysis') {
            steps {
                echo 'Stage 3 -- Code Analysis -- Tool: SonarQube Sonargate Check-- running'
                echo 'Stage 3 -- Code Analysis -- Tool: SonarQube Sonargate Check-- pass'
            }
        }

        stage('Security Scan') {
            steps {
                echo 'Stage 4 -- Security Scan -- Tool: OWASP Dependency-Check -- running'
                echo 'Stage 4 -- Security Scan -- Tool: OWASP Dependency-Check -- pass'
            }
        }

        stage('Deploy to Staging') {
            steps {
                echo 'Stage 5 -- Deploy to Staging -- Tool: AWS CLI -- running'
                echo 'Stage 5 -- Deploy to Staging -- Tool: AWS CLI -- pass'
            }
        }

        stage('Integration Tests on Staging') {
            steps {
                echo 'Stage 6 -- Integration Tests on Staging -- Tool: Postman (Newman CLI) -- running'
                echo 'Stage 6 -- Integration Tests on Staging -- Tool: Postman (Newman CLI) -- pass'
            }
        }

        stage('Deploy to Production') {
            steps {
                echo 'Stage 7 -- Deploy to Production -- Tool: AWS CLI -- running'
                echo 'Stage 7 -- Deploy to Production -- Tool: AWS CLI -- pass'
            }
        }
    }

    post {
        always {
            echo 'Pipeline execution completed.'
        }
    }
}
