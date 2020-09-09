
pipeline {
agent any
stages {
  stage('Build') {
    steps {
      slackUploadFile channel: 'https://hooks.slack.com/services/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', filePath: '/var/jenkins_home/workspace/slack/helloworld.html', initialComment: 'unit test'
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
}
