node {
  git url: 'https://github.com/cyrille-leclerc/multi-module-maven-project'
  withMaven {
    stage('Build'){
        sh 'mvn -B -DskipTests clean package'
    }
  }
}