pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Сборка проекта...'
                echo 'Имитация сборки завершена'
            }
        }

        stage('Test') {
            steps {
                echo 'Запуск тестов...'
                sh 'echo Тесты успешно пройдены'
            }
        }

        stage('Deploy') {
            steps {
                echo 'Развёртывание приложения...'
                sh 'echo Деплой выполнен'
            }
        }
    }

    post {
        always {
            echo 'Pipeline завершён'
        }
        success {
            echo 'Сборка прошла успешно'
        }
        failure {
            echo 'Ошибка выполнения pipeline'
        }
    }
}
