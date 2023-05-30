node {
    withDockerContainer(image: 'maven'){
    stage('Build'){
        sh 'mvn -B -DskipTests clean package'
    }
}
}