node {
    stage('checkout') {
        checkout scm
        println "Current branch ${BRANCH_NAME}"
    }
    stage('show-branch') {
        println "Current branch ${BRANCH_NAME}"
    }
    stage ('build') {
        sh 'mvn clean install'
    }
    stage('test') {
        sh 'mvn test'
    }
    stage('package') {
        sh 'mvn package'
    }
    stage('deploy') {
        sh 'mvn deploy -DskipTests'
    }
}
