node {
    withDockerContainer(args: '-u root', image: 'maven:latest'){
    stage('Build'){
        sh 'mvn -B -DskipTests clean package'
    }
    stage('Test'){
        sh 'mvn test'
        junit 'target/surefire-reports/*.xml'
        post {
          always {
           junit 'target/surefire-reports/*.xml'
          }
        }
    }
 }
}