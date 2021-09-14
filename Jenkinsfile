pipeline {
  agent any
  stages {
    stage('clone') {
      agent any
      steps {
        git(url: 'https://github.com/QANaveen/BlueOceanJenkins1.git', branch: 'main')
      }
    }

    stage('Build') {
      steps {
        bat 'mvn -f C:\\Users\\User\\.jenkins\\workspace\\BlueOceanJenkins1_main\\BlueOceanNew\\pom.xml test package'
      }
    }

  }
}