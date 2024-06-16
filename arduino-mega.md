# Arduino Mega

## LED Task

{% code title="Blink once in a second" lineNumbers="true" fullWidth="false" %}
```arduino
#define LED_PIN 13  

void setup()
{
  pinMode(LED_PIN, OUTPUT);
}

void loop()
{
  // turn the LED on (HIGH is the voltage level)
  digitalWrite(LED_PIN, HIGH);
  delay(1000); // Wait for 1000 millisecond(s)
  // turn the LED off by making the voltage LOW
  digitalWrite(LED_PIN, LOW);
  delay(1000); // Wait for 1000 millisecond(s)
}
```
{% endcode %}

<figure><img src=".gitbook/assets/LED.gif" alt=""><figcaption><p>Simulation of the LED task</p></figcaption></figure>

\#
