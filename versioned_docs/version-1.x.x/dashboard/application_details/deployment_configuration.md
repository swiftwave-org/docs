---
id: deployment_configuration
title: Deployment Configuration
sidebar_position: 7
---

In **Deployment Configuration** section, you can *scale up* or *scale down* the application.

![Deployment Configuration](/assets/1.x.x/application-deployment-configuration.png)

**Deployment Modes -**
- **Replicated Mode** - In this mode, you can specify the number of instances you want to run for the application.
- **Global Mode** - In this mode, each server of swiftwave will run one instance of the application.

> 📌 Note: Currently you can't change the deployment strategy of the application. **Replicated** mode is suitable for most of the applications. If you don't know what to choose, then choose **Replicated** mode.