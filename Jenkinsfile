pipeline {
  agent any
  stages {
    stage('��ȡ����') {
      steps {
        echo '����Ĭ�� Jenkins ����ȡ����'
      }
    }
    stage('����') {
      steps {
        sh 'mvn clean package'
      }
    }
  }
}
