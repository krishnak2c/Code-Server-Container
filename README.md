# deploy-code-server on Heroku & Railway 🚀

A collection of one-click buttons and scripts for deploying [code-server](https://github.com/cdr/code-server) to various cloud hosting platforms. The fastest way to get a code-server environment! ☁️

|                                                                                                                 | Name              | Type          | Lowest-Price Plan             | Deploy                                                  |
| --------------------------------------------------------------------------------------------------------------- | ----------------- | ------------- | ----------------------------- | ------------------------------------------------------- |
| [![Railway](img/logo/railway.png)](https://railway.app)                                                         | Railway           | Container     | Free, Shared CPU, 1 GB RAM 🚀 | [see guide](guides/railway.md)                          |
| [![Heroku](img/logo/heroku.png)](https://heroku.com)                                                            | Heroku            | Container     | Free, 1 CPU, 512 MB RAM       | [see guide](guides/heroku.md)                           |
| [![Coder](img/logo/coder.png)](https://coder.com/docs)                                                          | Coder             | Dev Workspace | For developer teams 👨🏼‍💻        | [read the docs](https://coder.com/docs)                 |

---

## code-server on a Container

- Deployed containers do not persist, and are often rebuilt
  - Containers can shut down when you are not using them, saving you money
  - All software and dependencies need to be defined in the `Dockerfile` or install script so they aren't destroyed on a rebuild. This is great if you want to have a new, clean environment every time you code
  - Most app platforms do not support running docker or virtual volume mounts in the container.
  - Storage may not be persistent. You may have to use [rclone](https://rclone.org/) to store your filesystem on a cloud service. Documented below:
  - [📄 Docs for code-server-deploy-container](deploy-container/)
