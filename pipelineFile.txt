node{
    stage{'preperation'}{
        git 'https://github.com/shrey-jain/maven-jenkins'
    }
    stage{'compile'}{
        sh label: '', script: 'mvn compile'
    }
    stage{'test'}{
        sh label: '', script: 'mvn test'
    }
    stage{'package'}{
        sh label: '', script: 'mvn package'
    }
    
}