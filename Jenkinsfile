pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Сборка проекта (имитация)'
            }
        }

        stage('Test') {
            steps {
                echo 'Подготовка и запуск тестов'
                sh 'chmod +x test.sh'
                sh './test.sh'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Подготовка и деплой'
                sh 'chmod +x deploy.sh'
                sh './deploy.sh staging'
            }
        }
    }
}
