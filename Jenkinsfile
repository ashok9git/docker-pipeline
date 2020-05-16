node {

    checkout scm

    docker.withRegistry('https://hub.docker.com', 'dockerhub') {

        def customImage = docker.build("tomcat-pipe")

        /* Push the container to the custom Registry
        customImage.push() */
        sh "docker tag tomcat-pipe ashok9dockhub/ashok_batch:tomcat-pipe"
        sh "docker push ashok9dockhub/ashok_batch:tomcat-pipe"
    }
}
