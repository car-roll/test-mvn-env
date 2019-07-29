def builds = [:]

builds['windows'] = {
    node {
        withEnv(['SKIP=true']) {
            sh 'echo $SKIP'
        }
    }
}
parallel builds
