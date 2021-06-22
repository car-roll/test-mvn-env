// def builds = [:]

// builds['windows'] = {
//     node {
//         withEnv(['SKIP=true']) {
//             checkout scm
//             sh 'echo $SKIP'
//             sh 'mvn compile'
//         }
//     }
// }
// parallel builds

script {
    node {
        checkout scm
//         def val = tm('${JSON, file="sample.json", expr="$.store.book[?(@.title == 'Moby Dick')].price"}')
        def val = tm('${JSON, file="sample.json", expr="$.store.book[?(@.price < 5)].price"}')
        echo "debug: $val"
    }
}
