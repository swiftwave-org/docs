---
id: generate-certificate
title: swiftwave tls generate-certificate
tags:
  - CLI
sidebar_position: 3
---

Generate TLS certificates for swiftwave endpoints

> This command generates TLS certificates for swiftwave endpoints.
	It's not for generating certificates for domain of hosted applications

### Usage

```
swiftwave tls generate-certificate [flags]
```

### Flags


| Flag   |       Type       | Default |     Mandatory       |          Description              |
|--------|------------------|---------|---------------------|-----------------------------------|
| --domain | string | <center>Will be picked from swiftwave configuration file, if not provided</center> | <center>❌</center> | Domain name for which to generate the SSL certificate from Let's Encrypt |

