# Raspberry Pi Installation #

The non-gui moteus library will work on a Raspberry Pi out of the box:

```
pip3 install moteus
```

However, neither pypi nor piwheels has a functioning pyside2 library,
which is needed for `moteus_gui`, and thus tview.  Fortunately, it is
packaged in Raspberry Pi OS.  To use that version, you can do the
following:

```
sudo apt install python3-pyside2* python3-serial python3-can python3-matplotlib python3-qtconsole
sudo pip3 install asyncqt importlib_metadata pyelftools
sudo pip3 install --no-deps moteus moteus_gui
```

# Running moteus_tool and tview #

pi3hat specific options for these tools are documented at https://github.com/mjbots/pi3hat/blob/master/docs/reference.md#usage-with-client-side-tools
