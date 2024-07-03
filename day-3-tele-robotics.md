# Day 3: Tele-Robotics

This material is designed as supplementary to the Day 3 Slides. You should not use this material without first reading the slides and trying out by yourself. Instead, refer to this material only if you encounter issues or bugs while following the slides.

Humidity & Temperature Sensor

<figure><img src=".gitbook/assets/image.png" alt=""><figcaption><p>Pins Mapping for DHT22 Sensor</p></figcaption></figure>

Please install library `DHT Sensor Library`, then running the code below:

{% code title="Humidity & Temp Sensor" lineNumbers="true" %}
```cpp
#include <Adafruit_Sensor.h>
#include <DHT.h>
#include <DHT_U.h>

#define DHTPIN 2      // Define the pin connected to the DHT sensor
#define DHTTYPE DHT22 // Define the type of DHT sensor (DHT11, DHT22, DHT21, etc.)

DHT dht(DHTPIN, DHTTYPE);

void setup() {
  Serial.begin(9600);
  Serial.println("DHT22 sensor test!");

  dht.begin();
}

void loop() {
  // Wait between readings
  delay(2000);

  // Read humidity
  float h = dht.readHumidity();
  // Read temperature as Celsius
  float t = dht.readTemperature();
  // Read temperature as Fahrenheit
  float f = dht.readTemperature(true);

  // Check if any reads failed
  if (isnan(h) || isnan(t) || isnan(f)) {
    Serial.println("Failed to read from DHT sensor!");
    return;
  }

  // Compute heat index in Fahrenheit and Celsius
  float hif = dht.computeHeatIndex(f, h);
  float hic = dht.computeHeatIndex(t, h, false);

  Serial.print("Humidity: ");
  Serial.print(h);
  Serial.print(" %\t");
  Serial.print("Temperature: ");
  Serial.print(t);
  Serial.print(" *C ");
  Serial.print(f);
  Serial.print(" *F\t");
  Serial.print("Heat index: ");
  Serial.print(hic);
  Serial.print(" *C ");
  Serial.print(hif);
  Serial.println(" *F");
}

```
{% endcode %}

