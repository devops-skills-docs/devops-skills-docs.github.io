## Turn off
### Using systemctl (system control)
```shell
sudo systemctl poweroff [--force | --force --force]
```
### Using cli tool
Shutdown now
```shell
sudo shutdown -h now
```
- Shutdown at 02:00 AM
    ```shell
    sudo shutdown 02:00 
    ```
- Shutdown in 10 minutes
    ```shell
    sudo shutdown +10 'Custom message'
    ```
- Reboot in 10 minutes
    ```shell
    sudo shutdown -r +10 'Custom message'
    ```

## Reboot 
### Using systemctl (system control)
```shell
sudo systemctl reboot [--force | --force --force]
```

### Using cli tool
```shell
sudo reboot
```