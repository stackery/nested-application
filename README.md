# Example Nested Application

This is an example stack that includes a top-level application as well as two nested applications (MyNestedApp and MyNestedApp2). The root application has its own `template.yaml` configuration file, as does each nested application, and they are each individually deployed during the CloudFormation deployment process.

Read more about nested applications in the [Stackery docs](https://docs.stackery.io/docs/using-stackery/nested-applications/).

Here is an overview of the files:

```text
.
├── MyNestedApp                        <-- Nested application
│   ├── src                            <-- Nested function source directory
│   │   └── NestedFunction
│   │       ├── README.md
│   │       ├── index.js
│   │       └── package.json
│   └── template.yaml                  <-- Nested SAM infrastructure-as-code template
├── MyNestedApp2                       <-- Another nested application
│   ├── src                            <-- Nested function source directory
│   │   └── NestedFunction
│   │       ├── README.md
│   │       ├── index.js
│   │       └── package.json
│   └── template.yaml                  <-- Nested SAM infrastructure-as-code template
├── README.md                          <-- This README file
├── deployHooks/                       <-- Directory for storing deployment hooks
├── .gitignore                         <-- Gitignore for Stackery
├── .stackery-config.yaml              <-- Default CLI parameters for root directory
├── src                                <-- Top-level function source directory
│   ├── TopLevelGetFunction
│   │   ├── README.md
│   │   ├── index.js
│   │   └── package.json
│   └── TopLevelPostFunction
│       ├── README.md
│       ├── index.js
│       └── package.json
└── template.yaml                      <-- Top-level SAM infrastructure-as-code template
```