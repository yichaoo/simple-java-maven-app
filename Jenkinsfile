pipeline {
    agent {
        docker {
            image 'maven:3-alpine'
            args '-v /root/.m2:/root/.m2'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn -f 代码/jhdxccip/pom.xml -B -DskipTests clean package'
            }
        }
    }
}