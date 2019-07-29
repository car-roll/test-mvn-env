def builds = [:]

builds['windows'] = {
    node {
        withEnv(['SKIP=true']) {
            checkout scm
            sh 'echo $SKIP'
            sh 'mvn compile'
        }
    }
}
parallel builds
