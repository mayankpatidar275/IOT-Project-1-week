#include <LiquidCrystal.h>
LiquidCrystal lcd(12, 11, 5, 4, 3, 2);

void setup() {
  lcd.begin(16, 2);
  lcd.print("THANKS TO");
  delay(1000);
  lcd.begin(16, 2);
  lcd.print("SKILLS NIGHT");
}

void loop() {
  lcd.setCursor(0, 1);
  lcd.print(millis()/100 - 10);
}
