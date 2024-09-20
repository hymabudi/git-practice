pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                git branch: 'main', url: 'https://github.com/hymabudi/git-practice.git'
            }
        }
        stage('budi') {
            steps {
                echo 'budi'
            }
        }
        stage('Deploy') {
            steps {
                withCredentials([aws(accessKeyVariable: 'AWS_ACCESS_KEY_ID', credentialsId: 'e3e76501-f223-4b7a-ab5e-43a18f62c6cd', secretKeyVariable: 'AWS_SECRET_ACCESS_KEY')]) {
    //   sh 'aws s3 cp . s3://athadubucket --recursive'
}
            }
        }
    }
}
