node{
  def remote = [:]
  remote.name = 'oraclevm'
  remote.host = '152.67.160.182'
  remote.user = 'opc'
  remote.password = 'Muzammil073#'
  remote.allowAnyHosts = true
  stage('Remote SSH') {
   // writeFile file: 'abc.sh', text: 'ls -lrt'
   // sshScript remote: remote, script: "abc.sh"
    sshCommand remote : remote, command: "pwd"
      sshCommand remote : remote, command: "cd /home"
    sshCommand remote : remote, command: "pwd"
      sshCommand remote : remote, command: "ls -lrt"
  }     
  stage('Remote SSH2') {
    //writefile file: 'abc.sh' , text: 'ls -lrt'
    // sshScript remote: remote, script: "abc.sh"
       sshCommand remote : remote, command: "sudo mkdir micro_steps"
        sshCommand remote : remote, command: "cd micro_steps"
    sshCommand remote : remote, command: "pwd"
  }
}
    
