pipeline {
    agent any

    tools {
        maven 'mymaven'
    }

    stages {

        stage('DevCompile') {
            steps {
                bat 'mvn compile'
            }
        }

        stage('CodeReview') {
            steps {
                bat 'mvn -P metrics pmd:pmd'
            }
        }

        stage('UnitTest') {
            steps {
                bat 'mvn test'
            }
        }

        stage('MetricCheck') {
            steps {
                bat 'mvn cobertura:cobertura -Dcobertura.report.format=xml'
            }
        }

        stage('Package') {
            steps {
                bat 'mvn package'
            }
        }

        stage('Deploy') {
            steps {
                bat 'echo Hello World'
            }
        }
    }

    post {
        success {
            echo 'Pipeline completed successfully.'
        }

        failure {
            echo 'Pipeline failed.'
        }
    }
}