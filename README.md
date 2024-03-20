# otodx-bootloader
Customizations to the nVidia Jetson Bootloader for OtoDx.

West is used to manage the multiple git repos needed for Jetson.
nVidia repos are used by default, but can fork and use
custom versions as needed by changing the west.yml files.

For more information on west and its manifests, visit
[Zephyr West Manifests](https://docs.zephyrproject.org/latest/develop/west/manifest.html)

## Install west
`pip3 install --user -U west`

### Make sure ~/.local/bin is at the front of your PATH to find west
`echo $PATH`

`PATH=$PWD/.local/bin:$PATH`

### Init the project to desired project_folder
`mkdir project_folder`

`cd project_folder`

`west init -m git@github.com:sradcliffe-nottinghamspirk/otodx-bootloader`

`west update`
