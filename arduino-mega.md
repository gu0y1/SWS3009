# Arduino Mega

## LED Task

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

<figure><img src=".gitbook/assets/LED.gif" alt=""><figcaption></figcaption></figure>
