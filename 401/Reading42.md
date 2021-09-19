# Get the last known location

- We can request the last known location of the user's device by using Google play services location API.

- Note: When your app is running in the background, access to location should be critical to the core functionality of the app and is accompanied with proper disclosure to users.

### Specify app permission
Apps whose features use location services must request location permissions, depending on the use cases of those features.

- Write the code in the oncreate method:
````
fusedLocationClient = LocationServices.getFusedLocationProviderClient(this);
fusedLocationClient.getLastLocation()
        .addOnSuccessListener(this, new OnSuccessListener<Location>() {
            @Override
            public void onSuccess(Location location) {
                // Got last known location. In some rare situations this can be null.
                if (location != null) {
                    // Logic to handle location object
                }
            }
        });
````
- The getLastLocation() method returns a Task that you can use to get a Location object with the latitude and longitude coordinates of a geographic location.

- The location object may be *null* when:
    1. Location is turned off in the device settings.
    2. The device never recorded its location, which could be the case of a new device or a device that has been restored to factory settings.
    3. there is no active Fused Location Provider client that has requested location after the services restarted.

###  Choose the best location estimate

1. `getLastLocation()`: gets a location estimate more quickly and minimizes battery usage that can be attributed to your app.
2. `getCurrentLocation()` gets a fresher, more accurate location more consistently. However, this method can cause active location computation to occur on the device.

### Resources
- [Locations](https://developer.android.com/training/location/retrieve-current)