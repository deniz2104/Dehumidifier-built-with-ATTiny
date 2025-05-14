# Dezumidificator cu ATTiny45 bazat pe o bucla de reglare

## Descriere

Acest proiect constă în realizarea unui dezumidificator automat care monitorizează umiditatea și ajustează viteza unui ventilator pentru a menține condițiile optime. Sistemul utilizează un microcontroler ATTiny45, un senzor de umiditate CJMCU-280, un afișaj LED cu 10 segmente pentru indicarea nivelului de umiditate și un ventilator DF1202512CL-087 controlat printr-o buclă de feedback.

## Funcționalități

- **Măsurarea umidității**: Senzorul CJMCU-280 detectează nivelul de umiditate din cameră.
- **Afișaj LED**: Un LED cu 10 segmente indică nivelul curent de umiditate.
- **Controlul ventilatorului**: Viteza ventilatorului DF1202512CL-087 este ajustată automat în funcție de umiditate:

  - La umiditate ridicată, ventilatorul va fi ajustat la o viteza ridicata.
  - Pe măsură ce umiditatea scade, viteza ventilatorului este redusă treptat până la un prag minim.

- **Buclă de feedback**: Sistemul ajustează continuu viteza ventilatorului pentru a menține umiditatea în limitele dorite.

## Proiecte Similare

1. **Humidity Sensor-Controlled Bathroom Exhaust Fan**

   - **URL**: ([Arduino Project Hub][1])
   - **Descriere**: Un proiect Arduino care utilizează un senzor DHT11 pentru a controla un ventilator de baie în funcție de umiditate. Ventilatorul pornește automat când umiditatea depășește un anumit prag.

2. **Humidity-Fan-Controller**

   - **URL**: ([GitHub][2])
   - **Descriere**: Un sistem bazat pe ESP32 care monitorizează temperatura și umiditatea folosind un senzor DHT22 și controlează un ventilator printr-un releu.([GitHub][2])

3. **Exhaust Fan Control**

   - **URL**: ([Arduino Project Hub][3])
   - **Descriere**: Un sistem care integrează senzori de temperatură, umiditate și gaze pentru a controla un ventilator de evacuare, oferind și alerte vizuale.

## Alte Detalii Relevante

- **Control PWM**: Viteza ventilatorului este ajustată prin semnal PWM generat de ATTiny45.
- **Alimentare**: Sistemul este alimentat la 5V.

[1]: https://projecthub.arduino.cc/LIMPINGLIM/humidity-sensor-controlled-bathroom-exhaust-fan-3b5d8b?utm_source=chatgpt.com "Humidity Sensor-Controlled Bathroom Exhaust Fan | Arduino Project Hub"
[2]: https://github.com/corrooli/Humidity-Fan-Controller?utm_source=chatgpt.com "GitHub - corrooli/Humidity-Fan-Controller: Simple ESP32-based fan controller for automatically triggering a AC fan when humidity reaches a threshold"
[3]: https://projecthub.arduino.cc/jiiroo19/exhaust-fan-control-c46e56?utm_source=chatgpt.com "Exhaust Fan Control | Arduino Project Hub"
