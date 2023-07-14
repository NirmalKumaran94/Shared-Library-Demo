pipeline {
    agent {
        agent "GIT"
    }
    stages  {
        stage GIT_HUB   {
            steps {
                githubTrigger()
            } 
        }
        stage Maven_Build   {
            steps {
                mavenBuild()
            } 
        }
        stage Nexus_Store   {
            steps {
                nexusStore()
            } 
        }
    }
}
