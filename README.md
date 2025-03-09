# Ansible Role: clickhouse
[![License](https://img.shields.io/badge/license-MIT%20License-brightgreen.svg)](https://opensource.org/licenses/MIT)

## Description

Deploy [Clickhouse](https://github.com/ClickHouse/ClickHouse) database system using ansible.

## Requirements

- Ansible >= 2.11 (It might work on previous versions, but we cannot guarantee it)
- Debian and python on deployer machine.

## Role Variables

All variables which can be overridden are stored in [defaults/main.yml](defaults/main.yml) file as well as in table below.

| Name           | Default Value | Description                        |
| -------------- | ------------- | -----------------------------------|
| `clickhouse_ver` | 22.3.3.44 | Clickhouse package version. Also accepts `latest` as parameter. |

## Example

### Playbook

```yaml
---
- name: CLICKHOUSE
  hosts: clickhouse
  roles:
    - role: clickhouse-role
      tags: clickhouse

```

## License

This project is licensed under MIT License. See [LICENSE](/LICENSE) for more details.


## Author Information

[ClickHouse](https://clickhouse.com/docs/en/index.html) by [ClickHouse, Inc.](https://clickhouse.com/company/).

Role by `Alex S`.