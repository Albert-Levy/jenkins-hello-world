pipeline {
    agent any

    stages {
        stage('Build Python') {
            steps {
                script {
                    // Commande pour exécuter le script Python
                    bat 'C:\\Users\\rehou\\AppData\\Local\\Microsoft\\WindowsApps\\python.exe hello.py'
                    
                    // Si vous voulez exécuter le script avec python3.exe à la place
                    // bat 'C:\\Users\\Albert\\AppData\\Local\\Microsoft\\WindowsApps\\python3.exe hello.py'
                }
            }
        }
        stage('Build Java') {
            steps {
                script {
                    // Commande pour compiler et exécuter le script Java
                    bat 'C:\\Program Files\\Common Files\\Oracle\\Java\\javapath\\javac.exe HelloWorld.java'
                    bat 'C:\\Program Files\\Common Files\\Oracle\\Java\\javapath\\java.exe HelloWorld'
                }
            }
        }
    }

    post {
        always {
            echo 'Pipeline finished!'
        }
    }
}
