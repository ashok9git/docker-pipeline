node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com/ashok9dockhub', 'dockerhub') {

        def customImage = docker.build("ashok_batch/tomcat-pipe")

        /* Push the container to the custom Registry */
        customImage.push()
    }
}
