node {
  withDockerContainer(image: 'maven:latest') {
    stage('Build'){
        sh 'mvn -B -DskipTests clean package'
    }
 }
}