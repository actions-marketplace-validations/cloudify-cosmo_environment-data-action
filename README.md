Retrieves a Cloudify environment's data, into a file and/or an output.

# Environment Variables

This Action uses the Cloudify Profile environment variables described in the official
Cloudify documentation (see [More Information](#more-information) below).

# Inputs

(Certain commonly-used inputs are documented in our official website; see [More Information](#more-information) below)

The environment's data is written into an output (`environment-data`).

If `outputs-file` is specified, then the environment's data is also written into that file.

# Example

```yaml
jobs:
  test_job:
    steps:
      - name: Get Environment Data
        uses: cloudify-cosmo/environment-data-action@v1.0
        with:
          environment-name: "my-environment"
          outputs-file: env-data.json
```

# More Information

Refer to [Cloudify CI/CD Integration](https://docs.cloudify.co/latest/working_with/integration/) for additional information about
Cloudify's integration with CI/CD tools.
