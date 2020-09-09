
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

      sh 'curl -F file=@/var/jenkins_home/workspace/slack/helloworld.html -H "Authorization: Bearer xoxp-1349477765779-1334528865959-1351909525091-face6d736a0b5e070f79bce4ad713584" -F channels=C01A9856B1Q https://slack.com/api/files.upload'

    }
    }

}
