pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                // Забираем код из репозитория
                git 'https://github.com/alexandrvolodin/ci-cd-demo.git'
            }
        }
        stage('Build') {
            steps {
                // Выполняем сборку
                echo 'Building project...'
                bat 'echo Building complete!'
            }
        }
        stage('Test') {
            steps {
                // Запускаем тесты
                echo 'Running tests...'
                bat 'echo Tests passed!'
            }
        }
        stage('Deploy') {
            steps {
                // Этап деплоя
                echo 'Deploying application...'
            }
        }
    }
}
