node {
    withDockerContainer(args: '-v /root/.m2:/root/.m2', image: 'maven:latest'){
    stage('Build'){
        sh 'mvn -B -DskipTests clean package'
    }
}
}