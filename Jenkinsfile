// trigger test

node {
    stage('checkout') {
        checkout scm
        println "Current branch ${BRANCH_NAME}"
    }
    stage ('build') {
        sh 'mvn clean install'
    }
    stage('deploy') {
        sh 'mvn jar:jar deploy:deploy'
    }
}
