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
import groovy.json.JsonOutput
script {
    node {
        checkout scm
//         def val = tm('${JSON, file="sample.json", expr="$.store.book[?(@.title == 'Moby Dick')].price"}')
//         def val = tm('${JSON, file="sample.json", expr="$.store.book[?(@.price < 5)].price"}')
        def val = tm('${JSON, file="sample.json", expr="$.project[version]"}')
//         def prettyJSON = JsonOutput.prettyPrint(val)
//         def prettyJSON = JsonOutput.prettyPrint(tm('${JSON, file="sample.json", expr="$.store.book[?(@.price < 5)].price"}'))
//         def prettyJSON = JsonOutput.prettyPrint(tm('${JSON, file="sample.json", expr="store"}'))
//         echo "${prettyJSON}"
    }
}
