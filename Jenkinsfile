node {
    stage('checkout') {
        git 'https://github.com/tcondit/spring-petclinic.git'
    }
    stage('compile-and-package') {
        def mvn_home = tool name: 'maven3', type: 'maven'
        sh "${mvn_home}/bin/mvn package"
    }
}
