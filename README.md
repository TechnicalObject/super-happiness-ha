# IMPORTANT: This action needs to be created in configuration.yaml

```yaml
action:
  - service: rest_command.healthchecks_ping
    data:
      project_uuid: "{{ project_uuid }}"
      healthcheck_slug: "{{ this.attributes.friendly_name | lower | replace(' ', '-') }}"
```
