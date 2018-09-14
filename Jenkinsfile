node {
    stage('checkout') { git 'https://github.com/tcondit/spring-petclinic.git' }
    stage('build')    { sh 'mvn clean install' }
    stage('test')     { sh 'mvn test' }
    stage('package')  { sh 'mvn package' }
    steps('deploy')   { sh 'mvn clean deploy -DskipTests' }
}
