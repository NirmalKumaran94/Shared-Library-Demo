pipeline {
    agent {
        agent 'GIT'
    }
    tools
    {
        maven ('maven_3.9.0')
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
        stage Clean_WorkSpace   {
            steps {
                cleanWS()
            } 
        }
    }
}
