# TaskGroupTemplates
A sample extension which installs TaskGroups to release management.

vss-extension.json skeleton 
```json
{
  "manifestVersion": 1,
  "id": "rm-tg-extensions2", // unqiue Id
  "version": "0.1.0",
  "name": "Sample Taskgroup1", // name of your task group extension
  "description": "Adds more tg templates to RM",  // sample description
  "publisher": "ms-devlabs",
  "public": true,
  "targets": [
    {
      "id": "Microsoft.VisualStudio.Services"
    }
  ],
  "screenshots": [
    {
      "path": "images/logo.png"
    }
  ],
  "content": {
    "details": {
      "path": "README.md"
    }
  },
  "icons": {
    "default": "images\\azureicon.png"
  },
  "contributions": [
    {
      "id": "sample-tgtemplate",
      "type": "ms.vss-taskgroup.tg-template",
      "targets": [
        "ms.vss-taskgroup.tg-templates"
      ],
      "properties": {
        "values": [
          {
            "tasks": [
              {
                
              }
            ]
          }
        ]
      }   // List of Task Groups (incase of nested, makesure the child task group is listed here)
    }
  ]
}
```
