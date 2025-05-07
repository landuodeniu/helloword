pipeline {
  agent any
  stages {
    stage('拉取代码') {
      steps {
        echo '这里默认 Jenkins 会拉取代码'
      }
    }
    stage('构建') {
      agent {
        docker {
            image 'maven:3.8.6-openjdk-11'  // 官方镜像
            args '-v $HOME/.m2:/root/.m2'    // 缓存Maven依赖到本地
        }
      }
      steps {
        sh 'mvn clean package'
      }
    }
  }
}
