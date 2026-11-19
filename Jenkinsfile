
pipeline {
    agent any

    options {
        timestamps()
    }

    stages {
        stage('Checkout Repository') {
            steps {
                echo 'Mengambil kode AI ROB dari GitHub'
                checkout scm
            }
        }

        stage('Pemeriksaan Repository') {
            steps {
                echo 'Repository AI ROB LAWU berhasil diakses'
                sh 'pwd'
                sh 'ls -la'
            }
        }

        stage('Status AI ROB') {
            steps {
                echo 'AI ROB LAWU GROUP SIAP DIKEMBANGKAN'
            }
        }
    }

    post {
        success {
            echo 'PIPELINE AI ROB BERHASIL'
        }
        failure {
            echo 'PIPELINE AI ROB GAGAL'
        }
    }
}
