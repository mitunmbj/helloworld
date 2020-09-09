
pipeline {
agent any
stages {
  stage('Build') {
    steps {
       sh 'echo "This is my Test step"'
    }
  }
  stage('Test') {
    steps {
      sh 'echo "This is my Test step"'
    }
  }
  stage('Deploy') {
    steps {
      sh 'echo "This is my Deploy step"'
    }
  }
}

post {
    always {
slackUploadFile channel: 'https://mbjinternational.slack.com/archives/C01A9856B1Q', credentialId: 'slack token', filePath: 'sample.html', initialComment: 'unittest'  
    }
    }

}
