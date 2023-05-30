node {
    withDockerContainer(args: '-u root', image: 'maven-alpine:latest'){
    stage('Build'){
        sh 'mvn -B -DskipTests clean package'
    }
    stage('Test'){
        sh 'mvn test'
        junit 'target/surefire-reports/*.xml'
        
    }
 }
}