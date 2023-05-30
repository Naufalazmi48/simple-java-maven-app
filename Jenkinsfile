node {
  withDockerContainer('maven') {
    stage('Build'){
        sh 'mvn -B -DskipTests clean package'
    }
 }
}