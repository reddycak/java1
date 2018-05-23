pipeline{
agent any
stages{
stage ('Compile Stage){
steps{
WithMaven(maven: 'maven_3_5_0'){
sh 'mvn clean compile'
}
}
}
stage ('Testing Stage'){
steps{
WithMaven(maven: 'maven_3_5_0){
sh 'mvn test'
}
}
}
stage ("Deploymwnt Stage'){
steps{
WithMaven(maven :'maven_3_5_0){
sh 'mvn deploy'
}
}
}
}
}
