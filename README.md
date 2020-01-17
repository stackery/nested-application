# Example Nested Application

This is an example stack that includes a top-level application as well as two nested applications (MyNestedApp and MyOtherNestedApp). The root application has its own `template.yaml` configuration file, as does each nested application, and they are combined during the deployment process.

Here is an overview of the files:

```text
.
├── deployHooks/                       <-- Directory for storing deployment hooks
├── .gitignore                         <-- Gitignore for Stackery
├── .stackery-config.yaml              <-- Default CLI parameters for root directory
├── README.md                          <-- This README file
└── template.yaml                      <-- Top-level SAM infrastructure-as-code template
```
