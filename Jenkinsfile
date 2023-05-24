node {
    stage('Checkout') {
        git 'https://github.com/MaheswariTAnisha/mghgyugu.git'
    }
    
    stage('Build') {
        bat 'mvn clean install'
    }
    
    stage('Test') {
        bat 'mvn test'
    }
    
    stage('Deploy') {
         bat 'xcopy target\\*.war "C:\\Program Files\\Apache Software Foundation\\Tomcat 9.0\\webapps"/Y'

    }
    
}
