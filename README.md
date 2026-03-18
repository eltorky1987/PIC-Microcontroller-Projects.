#include <xc.h>
#define _XTAL_FREQ 20000000

void main(void) {
    TRISB0 = 0; // Set RB0 as output
    while(1) {
        RB0 = 1; // LED ON
        __delay_ms(500);
        RB0 = 0; // LED OFF
        __delay_ms(500);
    }
}
