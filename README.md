# Send Message via WhatsApp
+ Code
    ```cpp
    #include "DigiKeyboard.h"
    
    void setup() {
      // Setting Pins
      pinMode(1, OUTPUT); // LED
      
      // Initialize DigiKeyboard
      DigiKeyboard.update();
      DigiKeyboard.delay(1000);
      
      // Goes to Home
      DigiKeyboard.sendKeyStroke(KEY_ENTER, MOD_GUI_LEFT); // Open Keyboard Shortcuts
      DigiKeyboard.delay(1000);
    
      DigiKeyboard.sendKeyStroke(KEY_Z, MOD_GUI_LEFT); // Goes to Home screen
      DigiKeyboard.delay(1000);
    
      DigiKeyboard.sendKeyStroke(43); // Press Tab
      DigiKeyboard.delay(1000);
    
      DigiKeyboard.sendKeyStroke(KEY_ENTER); // Enter
      DigiKeyboard.delay(1000);
      
      DigiKeyboard.print("apps");
      DigiKeyboard.delay(1000);
    
      DigiKeyboard.sendKeyStroke(KEY_ENTER); // Enter
      DigiKeyboard.delay(1000);
    
      DigiKeyboard.sendKeyStroke(81); // Down Arrow
      DigiKeyboard.delay(1000);
    
      DigiKeyboard.sendKeyStroke(KEY_ENTER); // Enter
      DigiKeyboard.delay(1000);
    
      DigiKeyboard.sendKeyStroke(43); // Tab
      DigiKeyboard.delay(1000);
    
      DigiKeyboard.sendKeyStroke(KEY_ENTER); // Enter
      DigiKeyboard.delay(1000);
    
      DigiKeyboard.print("Whatsapp\n"); // App
      DigiKeyboard.delay(1000);
    
      DigiKeyboard.sendKeyStroke(43); // Tab
      DigiKeyboard.sendKeyStroke(81); // Down
      DigiKeyboard.sendKeyStroke(81); // Down
      DigiKeyboard.delay(1000);
      
      DigiKeyboard.sendKeyStroke(KEY_ENTER); // Enter
      DigiKeyboard.delay(1000);
    
      DigiKeyboard.sendKeyStroke(43 , MOD_SHIFT_LEFT); // Shift + Tab
      DigiKeyboard.sendKeyStroke(43 , MOD_SHIFT_LEFT); // Shift + Tab
      DigiKeyboard.sendKeyStroke(43 , MOD_SHIFT_LEFT); // Shift + Tab
      DigiKeyboard.delay(1000);
    
      DigiKeyboard.sendKeyStroke(KEY_ENTER); // Enter
      DigiKeyboard.delay(1000);
    
      DigiKeyboard.sendKeyStroke(81); // Down arrow
      DigiKeyboard.sendKeyStroke(81); // Down arrow
      DigiKeyboard.delay(1000);
    
      DigiKeyboard.sendKeyStroke(KEY_ENTER); // Enter
      DigiKeyboard.delay(1000);
    
      DigiKeyboard.print("Hello, This is Semi-Automated Message\n\nKindly, Please go to my GitHub Repositories for more information https://github.com/dileep-kumar-koppula?tab=repositories"); // Message
      DigiKeyboard.delay(1000);
      
      DigiKeyboard.sendKeyStroke(43); // Tab
      DigiKeyboard.sendKeyStroke(43); // Tab
      DigiKeyboard.delay(500);
      
      DigiKeyboard.sendKeyStroke(KEY_ENTER); // Enter
      
      // Turn the LED ON
      digitalWrite(1, HIGH); // LED ON
    }
    
    void loop() {
      // No need for loop
    }
    ```
