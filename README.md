#include <LiquidCrystal.h>

LiquidCrystal lcd(8,9,10,11,12,13);//rs,e,D4,D5,D6,D7

void setup() {
 
  lcd.begin(16,2);
 
}

void loop() {
  lcd.setCursor(1,0);//(row,column)
   lcd.print("hello, world");
   lcd.setCursor(1,1);//(row,column)
   lcd.print("i'm elsa");
  delay(3000);
  lcd.clear();
  
    lcd.setCursor(2,0);//(row,column)
   lcd.print("this is a LCD");
  lcd.setCursor(2,1);
  lcd.print("screen test");
  delay(3000);
  lcd.clear();
 
}
