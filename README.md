# Serverlesspresso

This project aims to provide a coffee-ordering application inspired by
serverlesspresso. 

## Current status

The repository starts with an older snapshot of the serverlesspresso backend.
It is a reference baseline, not a modernized or deployment-ready application.
The original project has continued to evolve since this snapshot.

The snapshot contains AWS SAM infrastructure, backend services, and optional
extensions. It does not include the three frontend applications described by
the original project.

- `00-baseCore/` - foundational AWS resources, authentication, and messaging.
- `01-appCore/` - application infrastructure and initialization.
- `backends/` - coffee-ordering services and workflows.
- `extensions/` - optional example extensions.

Generated deployment exports were omitted from the import. Account-number-shaped
values in sample data and workflow definitions were replaced with
`000000000000`; review these placeholders before deploying.

## Validation and next steps

The imported JavaScript and JSON files passed syntax checks. The application
has not been deployed or functionally validated, and the AWS SAM CLI was not
available during the import. The snapshot references Node.js 14 and will need
modernization before deployment.

Future work can assess the current upstream project, modernize the backend,
and decide which ordering features and frontend applications to build.
Deploying AWS resources may incur charges.

For historical context, see the
[Serverlesspresso workshop](https://workshop.serverlesscoffee.com/).

## License

This repository retains the original [MIT-0 license](LICENSE), which permits
free use, modification, and distribution. The imported project includes
original copyright attribution in the license.
