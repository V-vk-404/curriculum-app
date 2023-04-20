pipeline {
  agent any
  stages {
    stage('Git Clone Repo') {
      steps {
        git(url: 'https://github.com/V-vk-404/curriculum-app.git', branch: 'dev')
      }
    }

    stage('FrontEnd-Unit-Test') {
      steps {
        sh 'cd curriculum-front && npm i && npm run test:unit'
      }
    }

  }
}