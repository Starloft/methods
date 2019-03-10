pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing Python combined solution'
                sh pytest --cov=projects/fizzbuzz/python/combined/ --cov-report=term-missing projects/fizzbuzz/python/combined/fizzbuzz_test.py
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}