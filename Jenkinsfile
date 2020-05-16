node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com/ashok9dockhub', 'dockerhub') {

        def customImage = docker.build("tomcat-pipe")

        /* Push the container to the custom Registry
        customImage.push() */
        sh "docker tag tomcat-pipe ashok9dockhub/ashok_batch:tomcat-pipe"
        sh "docker push ashok9dockhub/ashok_batch:tomcat-pipe"
    }
}
