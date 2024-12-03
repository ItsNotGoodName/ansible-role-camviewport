# ansible-role-camviewport

An Ansible Role that installs and configures [CamViewport](https://github.com/ItsNotGoodName/camviewport) on Debian based systems.

## Requirements

N/A

## Role Variables

N/A

## Role Tags

`camviewport_update` can be used to force update the binary.

## Dependencies

N/A

## Example Playbook

```yaml
- hosts: all
  roles:
    - itsnotgoodname.camviewport
```

## Display Output

Get list of display outputs.

```sh
sudo su camviewport -c 'DISPLAY=:0 xrandr'
```

Set display output, resolution, and fps.

```sh
sudo su camviewport -c 'DISPLAY=:0 xrandr --auto -s 1920x1080 -r 60'
```

Save the current display output as the default.

```sh
sudo su camviewport -c 'DISPLAY=:0 autorandr --save default --force'
```

## License

MIT

## Author Information

ItsNotGoodName
