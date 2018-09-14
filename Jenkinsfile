node {
    stage('checkout') { git 'https://github.com/tcondit/spring-petclinic.git' }
    stage('build')    { steps { sh 'mvn clean install' } }
    stage('test')     { steps { sh 'mvn test' } }
    stage('package')  { steps { sh 'mvn package' } }
    steps('deploy')   { steps { sh 'mvn clean deploy -DskipTests' } }
}
