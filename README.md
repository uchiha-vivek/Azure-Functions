## Azure Functions from beginner POV

<p align="center">
  <a href="https://github.com/uchiha-vivek/Azure-Functions">
    <img src="./assets/azure_functions.png" width="200" alt="ally" style="margin: 0 15px;" />
  </a>
  </p>

<h1 align="center">
  Azure Functions HTTP Trigger
</h1>


### Steps to create Azure Function from VS Code Locally

NOTE: you should have azure subscription

Download **Azure Tools extension pack for Visual Studio Code**


Make sure that you have host.json at the root level


**Zip** the entier azure function folder 

Inside azure cloud shell unzip it


Now run
```bash
func start
```

It will run like:
```bash
Functions:

   vivektrigger: [GET,POST] http://localhost:7071/api/vivektrigger

```

Test the endpoint in CURL
```bash
curl "http://localhost:7071/api/vivektrigger?name=Vivek"
```

OUTPUT 
```bash
Hello, Vivek. This HTTP triggered function executed successfully.
```

When we should use Azure functions:

- Scheduling Tasks
- For lightweight WEB API
- For different cron jobs
- Email Notification systems

[Docs for Reference](https://www.c-sharpcorner.com/article/why-and-when-to-use-azure-functions/)


## Next 2 projects i am working on

- Time based Trigger - sending email notifications everyday 2 times
- Webhook trigger with slack and gmail integrated