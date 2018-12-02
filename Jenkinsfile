podTemplate(
    label: 'mypod', 
    inheritFrom: 'default',
    containers: [
        containerTemplate(
            name: 'ubuntu', 
            image: 'ubuntu:latest',
            ttyEnabled: true,
            command: 'cat'
        )
    ]
) {
    node('mypod') {
        def passing_variable
        stage ('Assign') {
            passing_variable = "HELLO WORLD!"
        }
        stage ('Print') {
            container ('ubuntu') {
                sh 'echo $passing_variable'
            }
        }
    }
}
