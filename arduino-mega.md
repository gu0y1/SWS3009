# Arduino Mega

## LED Task

### Blink once in two seconds

This code is from Prof's slides. We implemented the LED connecting to GND and Pin 13 on Arduino to replicate the expected performace.

{% code title="Blink once in two seconds" lineNumbers="true" fullWidth="false" %}
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

<figure><img src=".gitbook/assets/LED.gif" alt=""><figcaption><p>Blink once in two seconds</p></figcaption></figure>

### Blink twice in a second

To make the LED blink twice in a second, you need to change the delay times to 250 milliseconds. This will ensure that the LED turns on and off twice within one second. Here's the modified code:

<pre class="language-arduino" data-title="Blink twice in a second" data-line-numbers><code class="lang-arduino"><strong>#define LED_PIN 13  
</strong>
void setup()
{
  pinMode(LED_PIN, OUTPUT);
}

void loop()
{
  // turn the LED on (HIGH is the voltage level)
  digitalWrite(LED_PIN, HIGH);
  delay(250); // Wait for 250 millisecond(s)
  // turn the LED off by making the voltage LOW
  digitalWrite(LED_PIN, LOW);
  delay(250); // Wait for 250 millisecond(s)
}
</code></pre>

<figure><img src=".gitbook/assets/LED2.gif" alt=""><figcaption><p>Blink twice in a second</p></figcaption></figure>

### Blink short-short-long

To make the LED blink in a short-short-long pattern, you can define the short and long delay times and sequence the blinks accordingly. Here's how you can achieve this:

{% code title="Blink short-short-long" lineNumbers="true" %}
```arduino
#define LED_PIN 13  

void setup()
{
  pinMode(LED_PIN, OUTPUT);
}

void loop()
{
  // Short blink
  digitalWrite(LED_PIN, HIGH);
  delay(250); // LED on for 250 milliseconds
  digitalWrite(LED_PIN, LOW);
  delay(250); // LED off for 250 milliseconds
  
  // Another short blink
  digitalWrite(LED_PIN, HIGH);
  delay(250); // LED on for 250 milliseconds
  digitalWrite(LED_PIN, LOW);
  delay(250); // LED off for 250 milliseconds
  
  // Long blink
  digitalWrite(LED_PIN, HIGH);
  delay(1000); // LED on for 1000 milliseconds (1 second)
  digitalWrite(LED_PIN, LOW);
  delay(1000); // LED off for 1000 milliseconds (1 second)

  // Pause before repeating the sequence
  delay(1000); // Pause for 1 second before repeating the pattern
}
```
{% endcode %}

In this code:

* A short blink is achieved with 250 milliseconds on and 250 milliseconds off.
* A long blink is achieved with 1000 milliseconds on and 1000 milliseconds off.
* A 1-second pause is added after the pattern to make it more distinguishable before it repeats.

<figure><img src=".gitbook/assets/LED3.gif" alt=""><figcaption></figcaption></figure>
