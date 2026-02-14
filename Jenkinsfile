pipeline {
    agent any
    
    stages {
       stage('Clone') {
    steps {
        git branch: 'main',
            url: 'https://github.com/SUNILKUMAR-12345/my-python-app-'
    }
}

        }
        
        stage('Build Docker Image') {
            steps {
                sh 'docker build -t python-app .'
            }
        }
        
        stage('Run Container') {
            steps {
                sh 'docker run -d -p 5000:5000 python-app'
            }
        }
    }
}
