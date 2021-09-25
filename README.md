# Jenkins Assignment

<!-- Create a Jenkins Job (Type Pipeline) which does the following: -->
  <summary><h2 style="display: inline-block">Create a Jenkins Job (Type Pipeline) which does the following:</h2></summary>
  All these steps should run on a Jenkins Slave:
  <details open="open">
  <ol>
    <li>
      Clones the PetClinic GitHub repository:
      <ul>
        https://github.com/spring-projects/spring-petclinic
      </ul>
    </li>
    <li>
      Builds the Job with the command lines:
      <ul>
        <li>git clone https://github.com/spring-projects/spring-petclinic.git</li>
        <li>cd spring-petclinic</li>
        <li>./mvnw package</li>
      </ul>
    </li>
    <li>Run the Application on the Jenkins Slave</li>
  </ol>
</details>

<!-- -->
## Results
### Pipeline pet-clinic Stage View
![stage view](https://user-images.githubusercontent.com/39053503/134781535-fdd554e3-9db2-4917-b80f-6bb9f1f31753.PNG)
 ## Status
 ![status](https://user-images.githubusercontent.com/39053503/134781595-498d0cd0-cd9a-4361-a6f5-77df5802f69f.PNG)
## Console Output
Started by user Assia Khateeb<br />
Obtained Jenkinsfile from git https://github.com/assiakhateeb/pet-clinic<br />
Running in Durability level: MAX_SURVIVABILITY<br />
[Pipeline] Start of Pipeline<br />
[Pipeline] node<br />
Running on slave in /home/ubuntu/jenkins/workspace/pet-clinic-pipeline<br />
[Pipeline] {<br />
[Pipeline] stage<br />
[Pipeline] { (Declarative: Checkout SCM)<br />
[Pipeline] checkout<br />
Selected Git installation does not exist. Using Default<br />
The recommended git tool is: NONE<br />
No credentials specified<br />
Fetching changes from the remote Git repository<br />
Checking out Revision d2c3fbc452e4921aa46036d7356f113d9939a3a3 (refs/remotes/origin/master)<br />
Commit message: "stage 3: Last Stage"<br />
 > git rev-parse --resolve-git-dir /home/ubuntu/jenkins/workspace/pet-clinic-pipeline/.git # timeout=10<br />
 > git config remote.origin.url https://github.com/assiakhateeb/pet-clinic # timeout=10<br />
Fetching upstream changes from https://github.com/assiakhateeb/pet-clinic<br />
 > git --version # timeout=10<br />
 > git --version # 'git version 2.25.1'<br />
 > git fetch --tags --force --progress -- https://github.com/assiakhateeb/pet-clinic +refs/heads/*:refs/remotes/origin/* # timeout=10<br />
 > git rev-parse refs/remotes/origin/master^{commit} # timeout=10<br />
 > git config core.sparsecheckout # timeout=10<br />
 > git checkout -f d2c3fbc452e4921aa46036d7356f113d9939a3a3 # timeout=10<br />
 > git rev-list --no-walk 077bbe36193b4205cf56b8a0b589fc078bfb7815 # timeout=10<br />
[Pipeline] }<br />
[Pipeline] // stage<br />
[Pipeline] withEnv<br />
[Pipeline] {<br />
[Pipeline] stage<br />
[Pipeline] { (Clone GitHub Repositry)<br />
[Pipeline] git<br />
The recommended git tool is: NONE<br />
No credentials specified<br />
Fetching changes from the remote Git repository<br />
Checking out Revision 25ba1621a9d7440df013f7737ce070f44014ecb1 (refs/remotes/origin/main)<br />
Commit message: "Add delimiter to list of pets"<br />
 > git rev-parse --resolve-git-dir /home/ubuntu/jenkins/workspace/pet-clinic-pipeline/.git # timeout=10<br />
 > git config remote.origin.url https://github.com/spring-projects/spring-petclinic # timeout=10<br />
Fetching upstream changes from https://github.com/spring-projects/spring-petclinic<br />
 > git --version # timeout=10<br />
 > git --version # 'git version 2.25.1'<br />
 > git fetch --tags --force --progress -- https://github.com/spring-projects/spring-petclinic +refs/heads/*:refs/remotes/origin/* # timeout=10<br />
 > git rev-parse refs/remotes/origin/main^{commit} # timeout=10<br />
 > git config core.sparsecheckout # timeout=10<br />
 > git checkout -f 25ba1621a9d7440df013f7737ce070f44014ecb1 # timeout=10<br />
 > git branch -a -v --no-abbrev # timeout=10<br />
 > git branch -D main # timeout=10<br />
 > git checkout -b main 25ba1621a9d7440df013f7737ce070f44014ecb1 # timeout=10<br />
 > git rev-list --no-walk 25ba1621a9d7440df013f7737ce070f44014ecb1 # timeout=10<br />
[Pipeline] }<br />
[Pipeline] // stage<br />
[Pipeline] stage<br />
[Pipeline] { (Change current directory)<br />
[Pipeline] dir<br />
Running in /home/ubuntu/jenkins/workspace/pet-clinic-pipeline/spring-petclinic<br />
[Pipeline] {<br />
[Pipeline] }<br />
[Pipeline] // dir<br />
[Pipeline] }<br />
[Pipeline] // stage<br />
[Pipeline] stage<br />
[Pipeline] { (Last Stage)<br />
[Pipeline] script<br />
[Pipeline] {<br />
[Pipeline] }<br />
[Pipeline] // script<br />
[Pipeline] }<br />
[Pipeline] // stage<br />
[Pipeline] }<br />
[Pipeline] // withEnv<br />
[Pipeline] }<br />
[Pipeline] // node<br />
[Pipeline] End of Pipeline<br />
Finished: SUCCESS<br />
