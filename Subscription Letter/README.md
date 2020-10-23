# Astro Pi subscription: CHIP Team



#### A)  Describe your team's experiment and what they plan to investigate.

Things in the world are getting worse and worse. Wildfires, floods, deforestation, and abnormal climate are destroying the environment. Our future is in danger, and we will prove it. We’ll investigate past data to create an algorithm able to supervise human activity and predict future environmental disasters.

We want to help humanity to safeguard the future of our planet. We now have weapons to fight against climate changes such as Artificial Intelligence and Machine Learning. We'll collect data mainly from the near-infrared camera. We plan to [parse](https://github.com/CHIP-AstroPi/docs/tree/master/phase1#23-satellite-imagery-parsing) in real-time the collected imagery and store them with the extracted data. We'll run the parsing process on historic satellite imagery and use the obtained data, with the ones coming from the Izzy real-time elaboration, to elaborate a statistical model able to "predict" the future impact. Our program will run various classification and detection algorithms on the captured images. We intend to detect as many elements as we can, starting from a few mandatory ones:

- Vegetation, hence
  
  - Desertification
  -  Forests

- Water, hence
  
  -  Lakes
  -  Rivers
  - Glaciers

- Coastlines, hence
  
  -  Sea level

| Algorithm            | Elements detected |
| -------------------- | ----------------- |
| NDVI                 | Vegetation        |
| NDWI                 | Water             |
| Coastlines detection | Coastlines        |

We want to make a difference.

For ourselves, for humanity.



#### B) What type of data does your team plan to gather?

Our experiment should be based only on satellite imagery from the Izzy camera, but we plan to collect magnetic field data as well to amplify our possibilities in the elaboration phase.

Sensor we will use to collect data:

- Izzy camera with blue filter

- Magnetometer
