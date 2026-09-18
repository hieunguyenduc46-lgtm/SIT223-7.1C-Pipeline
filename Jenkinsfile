pipeline {
    agent any

    stages {
        stage('1. Build') {
            steps {
                echo 'Stage 1: Build'
                echo 'Task: Compile the source code and package it into a deployable artifact such as a JAR or WAR file.'
                echo 'Tool: Maven'
            }
        }

        stage('2. Unit and Integration Tests') {
            steps {
                echo 'Stage 2: Unit and Integration Tests'
                echo 'Task: Run unit tests to verify individual components and integration tests to verify that the components work together correctly.'
                echo 'Tool: JUnit for unit tests and Selenium for integration tests'
            }
        }

        stage('3. Code Analysis') {
            steps {
                echo 'Stage 3: Code Analysis'
                echo 'Task: Analyse the source code to ensure it meets industry coding standards and to detect code smells and maintainability issues.'
                echo 'Tool: SonarQube'
            }
        }

        stage('4. Security Scan') {
            steps {
                echo 'Stage 4: Security Scan'
                echo 'Task: Scan the code and its dependencies to identify known vulnerabilities before deployment.'
                echo 'Tool: OWASP Dependency-Check'
            }
        }

        stage('5. Deploy to Staging') {
            steps {
                echo 'Stage 5: Deploy to Staging'
                echo 'Task: Deploy the built application to the staging server for pre-production verification.'
                echo 'Tool: AWS CLI deploying to an AWS EC2 staging instance'
            }
        }

        stage('6. Integration Tests on Staging') {
            steps {
                echo 'Stage 6: Integration Tests on Staging'
                echo 'Task: Run integration tests on the staging environment to confirm the application behaves correctly in a production-like setup.'
                echo 'Tool: Selenium'
            }
        }

        stage('7. Deploy to Production') {
            steps {
                echo 'Stage 7: Deploy to Production'
                echo 'Task: Deploy the verified application to the production server to make it available to end users.'
                echo 'Tool: AWS CLI deploying to an AWS EC2 production instance'
            }
        }
    }
}