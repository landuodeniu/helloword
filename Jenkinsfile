pipeline {
  agent any
  stages {
    stage('拉取代码') {
      steps {
        echo '这里默认 Jenkins 会拉取代码'
      }
    }
    stage('构建') {
      steps {
        sh 'mvn clean package'
      }
    }
  }
}
