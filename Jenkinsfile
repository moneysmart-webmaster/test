node {
    try {
        stage ('Staging') {
            sh "echo 'Deploy to Staging'"
        }
        stage ('PreProduction') {
            sh "echo 'Deploy to PreProduction'"
        }
    } catch (err) {
        currentBuild.result = 'FAILED'
        throw err
    }
}
