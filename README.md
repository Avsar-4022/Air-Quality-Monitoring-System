# Arduino-UNO Air-Quality Monitor  
This project turns an Arduino Uno into a simple air-quality station by combining an MQ-2 sensor (smoke/CO), an MQ-135 sensor (general air pollutants/PM₂.₅) and a DHT11 (temperature & humidity). It continuously reads gas and environment data, converts raw voltages into meaningful concentrations (ppm and µg/m³), and tags each value with a user-friendly label (Good, Moderate, Unhealthy, etc.).

After a one-time calibration to find each sensor’s clean-air resistance (R₀), the sketch measures sensor resistance in actual air, computes concentration via log-log formulas and converts it to µg/m³. All results—temperature, humidity, CO and PM₂.₅ levels plus their air-quality remarks—are streamed live to the Serial Monitor for quick viewing.
