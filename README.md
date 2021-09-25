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
