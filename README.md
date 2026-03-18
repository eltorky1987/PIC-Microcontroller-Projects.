#include <xc.h>
#define _XTAL_FREQ 20000000

void main(void) {
    TRISB0 = 0; // تعيين الطرف كمخرج
    while(1) {
        RB0 = 1; // تشغيل
        __delay_ms(500);
        RB0 = 0; // إطفاء
        __delay_ms(500);
    }
}
