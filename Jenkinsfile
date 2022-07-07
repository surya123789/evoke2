podTemplate(containers: [
    containerTemplate(
        name: 'jnlp', 
        image: 'surya123789/jenkins_slave:latest'
        )
  ]) {

    node(surya) {
        stage('Get a Maven project') {
            container('jnlp') {
                stage('Shell Execution') {
                    sh '''
                    echo "mvn package"
                    '''
                }
            }
        }

    }
}
