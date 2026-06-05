# Nitro Schema Download

A GitHub Action that downloads a GraphQL schema from a stage in the Nitro registry.

## Usage

```yaml
- uses: ChilliCream/nitro-schema-download@v16
  with:
    api-id: <api-id>
    stage: <stage>
    file: ./schema.graphql
    api-key: <api-key>
    # Optional
    cloud-url: <cloud-url>
```

## Inputs

| Name        | Required | Description                                     |
| ----------- | -------- | ----------------------------------------------- |
| `api-id`    | Yes      | The ID of the API                               |
| `stage`     | Yes      | The name of the stage                           |
| `file`      | Yes      | The file where the schema will be downloaded to |
| `api-key`   | Yes      | API key for authentication                      |
| `cloud-url` | No       | The URL of the Nitro registry                   |

If you self-host Nitro or use a dedicated hosted instance, you can specify the `cloud-url` input to point to your instance.
