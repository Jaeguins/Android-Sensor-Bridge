# Android-Sensor-Bridge
Bridge package between Unity &amp; Android for reading sensors for private use.

## Usages

### Namespace SensorReader

#### Class SensorReaderLibWrapper <br>
Bridge class for android parts.
 ##### `static void Initialize(void)` : <br>
 Initialize method. call this only one in starting.
 ##### `static string Start(SensorType type)` : <br>
 Try to start tracking `type` and return result.
 ##### `static string End(SensorType type)` : <br>
 Try to end tracking `type` and return result.
 ##### `static bool IsRunning(SensorType type)` : <br>
 Check `type` sensor is tracked now.
 ##### `static float Get(SensorType type,int index)` : <br>
 Try to Get Value of `type` sensor's `index` value. <br>
 Most sensors only useful `0`, but some are not.(ex. linear accelerometer)
#### Enum SensorType <br>
Sensor Type same defined in Android Sensor class. <br>
All values are same in Android reference <br>
   * `Accelerometer`
   * `MagneticField`
   * `Orientation` - deprecated
   * `Gyroscope`
   * `Light` - confirmed
   * `Pressure`
   * `Temperature` - deprecated
   * `Proximity`
   * `Gravity`
   * `LinearAcceleration`
   * `RotationVector`
   * `RelativeHumidity`
   * `AmbientTemperature`
   * `MagneticFieldUncalibrated`
   * `GameRotationVector`
   * `GyroscopeUncalibrated`
   * `SignificantMotion`
   * `StepDetector`
   * `StepCounter`
   * `GeomagneticRotationVector`
   * `HeartRate`
   * `AccelerometerUncalibrated`
   * `DevicePrivateBase`
   * `LowLatencyOffBodyDetect`
   * `MotionDetect`
   * `Pose6Dof`
   * `StationaryDetect`
   * `HeartBeat`
   * `All`
