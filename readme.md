# About

I thought it would be neat to get the RGB LEDs in my Corsair keyboard and mouse to copy or mirror what is on-screen (a bit like Sony Bravia TVs that have a backlight that changes according to what's on-screen). 

Turns out Corsair have a python SDK for iCue (https://github.com/CorsairOfficial/cue-sdk-python) so this is my first attempt. I'm surprised with how well it worked! 

I have an MSI motherboard and want to eventually apply the same principle, but I can only find the MSI Mystic Light SDK in C++ or C#. I'm not familiar with either, but I'd hope to be able to handle the main computation in python and import/export led values. Tbc, will be a while before I look into that. 

# How it works

- Take a screenshot (currently hard-coded to do this at 30 Hz), downscales to something tiny to pixelate the image, then upscales to image to the same dimensions of the keyboard + mouse. 
- Use device led cooridnates to sample the colour of the pixelated image.
- Apply colours to LEDs. 

#### Hardware:
- K68 RGB
- SABRE RGB

#### Python Library Dependancies:
- Numpy
- Pandas
- Corsair iCue SDK (python)
- Pillow (PIL)

#### Software Dependancies:
- Corsair iCue

# Examples

![text](./examples/ror2.jpg)
![text](./examples/ror2-intro.jpg)
![text](./examples/desktop.jpg)


```python

```
