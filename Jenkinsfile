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
                // Выполняем сборку (можно использовать различные команды в зависимости от проекта)
                echo 'Building project...'
                sh 'echo Building complete!'
            }
        }
        stage('Test') {
            steps {
                // Запускаем тесты (в данном случае просто имитируем)
                echo 'Running tests...'
                sh 'echo Tests passed!'
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
