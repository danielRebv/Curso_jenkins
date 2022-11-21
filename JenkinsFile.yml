node {
    
    stage('LimpiarEspacio de trabajo') { 
        cleanWs()
       
    }
    stage('Git') {
        git branch: 'main', url: 'https://github.com/danielRebv/Curso_jenkins.git'
      }
    
    stage('Compilacion maven') {
        sh 'mvn clean package'
    }
    stage('Pruebas Unitarias'){
        sh 'mvn test'
    }
}
