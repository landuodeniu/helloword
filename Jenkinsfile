pipeline {
  agent any
  stages {
    stage('��ȡ����') {
      steps {
        echo '����Ĭ�� Jenkins ����ȡ����'
      }
    }
    stage('����') {
      agent {
        docker {
            image 'maven:3.8.6-openjdk-11'  // �ٷ�����
            args '-v $HOME/.m2:/root/.m2'    // ����Maven����������
        }
      }
      steps {
        sh 'mvn clean package'
      }
    }
  }
}
