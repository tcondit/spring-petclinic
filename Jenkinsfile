//node {
//    stage('checkout') { git 'https://github.com/tcondit/spring-petclinic.git' }

    stage 'Init'
    node {
        checkout scm
        sh 'echo $BRANCH_NAME'
    }
    if (env.BRANCH_NAME == 'master') {
        stage 'Only on master'
        println 'This happens only on master'
    } else {
        stage 'Other branches'
        println "Current branch ${env.BRANCH_NAME}"
        println "Current branch ${BRANCH_NAME}"
    }

//    stage('branch')   { sh 'git checkout develop' }
//    stage('build')    { sh 'mvn clean install' }
//    stage('test')     { sh 'mvn test' }
//    stage('package')  { sh 'mvn package' }
//    stage('deploy')   { sh 'mvn deploy -DskipTests' }
//}
