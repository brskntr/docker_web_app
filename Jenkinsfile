node {
    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerHub') {

        def customImage = docker.build("bariskantar/docker_web_app")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
