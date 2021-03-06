# [Sensor device driver design guide](index.md)
# [What's New In Sensors](what-s-new-in-sensors.md)
# [Universal sensor driver model for Windows 10](converged-sensor-driver-model-for-windows-10.md)
## [Design Guide](design-guide.md)
### [Overview of universal sensor driver model](overview-of-converged-sensor-driver-model.md)
### [Windows sensor driver features](windows-sensor-driver-features.md)
#### [Sensor data batching for power savings](sensor-batching-for-power-saving-.md)
#### [Sensors ACPI entries](sensors-acpi-entries.md)
## [Programming Guide](programming-guide-v2.md)
### [How to build a universal sensor driver](how-to-build-a-universal-sensor-driver.md)
#### [Set up your development environment](set-up-your-development-environment.md)
#### [Prepare your sensor test board](prepare-your-sensor-test-board.md)
#### [Connect your sensor to the Sharks Cove board](connect-your-sensor-to-the-sharks-cove-board.md)
#### [Write and deploy your universal sensor driver](write-and-deploy-your-universal-sensor-driver.md)
##### [Make the driver loadable](make-the-driver-loadable.md)
##### [Connect to hardware](connect-to-hardware.md)
##### [Read data from hardware](read-data-from-hardware.md)
##### [Review the INX file](review-and-revise-the-inf-file.md)
###### [Creating a mobile package](creating-a-mobile-package.md)
##### [Build the sensor driver](build-the-sensor-driver.md)
##### [Install the sensor driver](install-the-sensor-driver.md)
#### [Test your universal sensor driver](test-your-universal-sensor-driver.md)
#### [Collecting and decoding WPP logs](collecting-and-decoding-wpp-logs.md)
### [Fusion sensor implementation details](fusion-sensor-implementation-details.md)
# [Sensor driver model for Windows 8.1](sensor-driver-model-for-windows-8-1.md)
## [New sensor features and improvements for Windows 8.1](new-sensor-features-and-improvements-for-windows-8-1.md)
## [Design Guide](sensor-driver-design-guide.md)
### [Getting Started](getting-started.md)
#### [Introduction to the Sensor and Location Platform in Windows](introduction-to-the-sensor-and-location-platform-in-windows.md)
#### [For More Information](for-more-information.md)
### [Sensor Driver Overview](sensor-driver-overview.md)
#### [Architecture Overview](architecture-overview-for-sensor-drivers.md)
#### [About the Sensor Class Extension](about-the-sensor-class-extension.md)
#### [About the Interfaces](about-the-interfaces.md)
##### [About ISensorClassExtension](about-isensorclassextension.md)
##### [About ISensorDriver](about-isensordriver.md)
##### [About the Parameter Types](about-the-parameter-types.md)
#### [About Sensor Driver Events](about-sensor-driver-events.md)
#### [About Sensor Constants](about-sensor-constants.md)
## [Programming Guide](programming-guide.md)
### [Sensor driver development basics](sensor-driver-development-basics.md)
#### [Writing a sensor device driver](writing-a-sensor-device-driver.md)
##### [Considerations for writing a sensor driver](considerations-for-writing-a-sensor-driver.md)
##### [Creating a sensor driver](creating-the-driver.md)
##### [Creating a persistent unique identifier for a sensor](creating-a-persistent-unique-identifier.md)
##### [Raising sensor events](raising-events.md)
##### [Filtering data](filtering-data.md)
##### [Using vector types with sensors](using-vector-types.md)
##### [Defining custom values for sensor constants](defining-custom-values-for-constants.md)
##### [Specifying a sensoricon](specifying-an-icon.md)
##### [Sensor driver best practices](sensor-driver-best-practices.md)
#### [Supporting ambient light sensors](supporting-ambient-light-sensors.md)
### [Sensor driver logic](driver-logic--pseudo-code-.md)
#### [Driver initialization methods](driver-initialization-methods.md)
#### [Driver interface methods](driver-interface-methods.md)
#### [Driver update methods](internal-helper-methods.md)
#### [Device update methods](device-update-methods.md)
#### [Internal driver methods](internal-driver-methods.md)
#### [Device methods](device-methods.md)
### [Testing sensor functionality with the Sensor Diagnostic Tool](the-sensor-diagnostic-tool.md)
#### [Testing Sensor Functionality](testing-sensor-functionality.md)
##### [Testing Sensor Events](testing-sensor-events.md)
##### [Testing Sensor Data Retrieval](testing-sensor-properties.md)
##### [Testing Sensor Property Support](testing-and-logging-sensor-data.md)
#### [Testing Location Functionality](testing-location-functionality.md)
#### [Known issues](known-issues.md)
### [SpbAccelerometer driver sample](spbaccelerometer-driver-sample.md)
#### [Supporting multiple sensors](supporting-multiple-sensors.md)
#### [The driver I/O model](the-driver-i-o-model.md)
#### [Defining the accelerometer object](defining-the-accelerometer-object.md)
#### [Using the sensor class extension](using-the-sensor-class-extension.md)
#### [Supporting the accelerometer properties](supporting-the-accelerometer-properties.md)
#### [The driver sample file list](the-driver-sample-file-list.md)
## [SpbAccelerometer driver cookbook](spbaccelerometer-driver-cookbook.md)
### [Install the sample device and driver on your Sharks Cove board](installing-the-sample-device-and-driver-on-your-sharks-cove-board.md)
### [SpbAccelerometer driver overview](spbaccelerometer-driver-overview.md)
### [Sample driver I/O model](the-sample-driver-i-o-model.md)
### [I2C transport](the-i2c-transport.md)
### [Accelerometer object](the-accelerometer-object.md)
### [Access the sensor class extension](accessing-the-sensor-class-extension.md)
### [Support for device  properties](supporting-the-device--properties.md)
### [Driver initialization](driver-initialization.md)
### [Modify the sample to support another sensor](modifying-the-sample-to-support-another-sensor.md)
### [Use the Sensors Diagnostic Tool to test your driver and device](using-the-sensors-diagnostic-tool-to-test-your-driver-and-device.md)

