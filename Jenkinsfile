node {
    stage('checkout') { git 'https://github.com/tcondit/spring-petclinic.git' }
    stage('branch')   { sh 'git checkout develop' }
    stage('build')    { sh 'mvn clean install' }
    stage('test')     { sh 'mvn test' }
    stage('package')  { sh 'mvn package' }
    stage('deploy')   { sh 'mvn deploy -DskipTests' }
}
