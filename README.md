# IMPORTANT: This action needs to be created in configuration.yaml

```yaml
rest_command:
  healthchecks_ping:
    url: >-
      https://hc.casp.run/ping/{{ project_uuid | default(states('input_text.healthchecks_uuid')) }}/{{ healthcheck_slug | default('') }}{{
        ping_type | default('')
      }}
```
