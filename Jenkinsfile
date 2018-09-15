stage 'checkout' {
    node {
        checkout scm
        println "Current branch ${BRANCH_NAME}"
//        sh 'echo Current branch is $BRANCH_NAME'
    }
}

stage 'show-branch' {
    println "Current branch ${BRANCH_NAME}"
}

//    stage('branch')   { sh 'git checkout develop' }
//    stage('build')    { sh 'mvn clean install' }
//    stage('test')     { sh 'mvn test' }
//    stage('package')  { sh 'mvn package' }
//    stage('deploy')   { sh 'mvn deploy -DskipTests' }
//}
