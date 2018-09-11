# Dimirtos personal overlay

Some embedded and wiki stuff will be placed here

## Warning

Use at your own risks

## Installation

### Using layman

#### Install layman
    1. emerge layman
    
    
    2. Configure layman to use the repos.conf method in /etc/layman/layman.cfg. New installations of layman will probably have this already set correctly:
    FILE /etc/layman/layman.cfg

    # Repository config types used by layman
    # (repos.conf, make.conf)
    conf_type : repos.conf

#### Add the 'dimirtost' overlay
    layman -o https://github.com/irtos/overlay_irtos/raw/master/overlay.xml -f -a dimirtos

#### Sync overlays
    layman -S

#### Install
    emerge package_name