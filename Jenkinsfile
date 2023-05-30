node {
    withDockerContainer(args: '-u root', image: 'maven:3.6.3-jdk-8'){
    stage('Build'){
        sh 'mvn -B -DskipTests clean package'
    }
    stage('Test'){
        sh 'mvn test'
    }
 }
}