node {

    checkout scm

    docker.withRegistry('https://crepantherx.jfrog.io/artifactory/docker/', 'jfrog') {

        def customImage = docker.build("docker/apper")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
