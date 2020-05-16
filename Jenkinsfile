node {

    checkout scm

    docker.withRegistry('https://registry.hub.docker.com', 'dockerhub') {

        def customImage = docker.build("ashok9dockhub/ashok_batch")

        /* Push the container to the custom Registry*/
        customImage.push("tomcat9")
        /*sh "docker tag tomcat-pipe ashok9dockhub/ashok_batch:tomcat-pipe"
        sh "docker push ashok9dockhub/ashok_batch:tomcat-pipe"*/
    }
}
