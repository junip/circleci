# Circle CI <img src="https://img.shields.io/badge/Circle-CI-green" />

Circle CI build configuration details.
Easy to checkout config details Repo. 

<details>
  <summary>Table Of Content</summary>
</details>

<br/>
<br/>
<br/>

### Start your first CI
- create a folder `.circleci`
- create a file `config.yml` inside the `.circleci` folder.
- add the configuration and pushed the code. 

### Version 
- Need to specify the version before use
- to use `Orbs` need to specify the version `2.1`

### Orbs (requires version: 2.1)
- its a package that contains few commands definations that are reusable for the builds.
- its a parameterizable elements, including jobs, commands, and executors.

### Commands (requires version: 2.1)
- Commands are the sequence of steps run inside the calling job of the command.

### Parameters (requires version: 2.1)
- used in jobs steps declarations etc

### Jobs
- A Workflow is comprised of one or more uniquely named jobs.
- jobs are the task to perform in a CI builds.

### Commands 
- commands are the instruction to execute for a job



# CLI Commands

### validate `yml` configurations
```
circleci config validate
```


