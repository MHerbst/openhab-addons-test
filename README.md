# Install the test add-on

1. Uninstall the Homematic binding 
1. Stop openHAB
1. Clean the cache
1. Copy the test jar into the `addons` folder
1. Start openHAB (on slow devices like Raspberry you have to start openHAB a second time because of the emptied cache)

If the binding does not start, you may have to install manually two additional bundles via the Karaf console:

```
feature:install openhab-transport-upnp
feature:install openhab-transport-serial
```