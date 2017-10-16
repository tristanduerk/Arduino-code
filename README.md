# Arduino-code
#include <Adafruit_NeoPixel.h>

#ifdef AVR

#include <avr/power.h>

#endif

int const NUM_PIXELS = 12;

int8_t const PIN = 13;

Adafruit_NeoPixel strip;

int num = 0;

void setup() {

strip = Adafruit_NeoPixel(NUM_PIXELS, PIN, NEO_GRB+NEO_KHZ800);

strip.begin();

strip.show(); 
}

void loop() { for(int i = 0; i < NUM_PIXELS; i++) {

  strip.setPixelColor(i, 0xFFF012);
  
  strip.show();
  
  delay(50);
}
  strip.setPixelColor(i, 0xFF0000);
  strip.show();
  
  strip.setPixelColor(1, 0xFF0000);
  
  strip.setPixelColor(2, 0x00FF00);
  
  strip.setPixelColor(3, 0x0000FF);
  
  strip.setPixelColor(4, 0xFFFF00);
  
  strip.setPixelColor(5, 0xBB33FF);
  
  strip.setPixelColor(6, 0x33FCFF);
  
  strip.setPixelColor(7, 0x55FFAA);
  
  strip.setPixelColor(8, 0xFF9633);
  
  strip.setPixelColor(9, 0x9633FF);
  
  strip.setPixelColor(10, 0x33FFE6);
  
  strip.setPixelColor(11, 0xFF3369);
  
  strip.setPixelColor(12, 0x33FFA5)
}
strip.show();
}
