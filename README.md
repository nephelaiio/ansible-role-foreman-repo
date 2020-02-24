# nephelaiio.foreman_repo

Install foreman repositories

## Role Variables

| required | variable        | description                             | default |
| ---      | ---             | ---                                     | ---     |
| *no*     | foreman_release | foreman release for included repository | 1.24    |

## Example Playbook

```
    - hosts: foreman
      roles:
         - role: nephelaiio.foreman_repo
           vars:
             foreman_release: 1.24
             ```

## Testing

Please make sure your environment has [docker](https://www.docker.com) installed in order to run role validation tests. Additional python dependencies are listed in the [requirements file](https://github.com/nephelaiio/ansible-role-requirements/blob/master/requirements.txt)

Role is tested against the following distributions (docker images):
  * Ubuntu Bionic
  * CentOS 7

You can test the role directly from sources using command ` molecule test `

## License

This project is licensed under the terms of the [MIT License](/LICENSE)
