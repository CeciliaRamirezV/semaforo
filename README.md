# semaforo
void main()
{

   setup_adc_ports(NO_ANALOGS);
   setup_adc(ADC_CLOCK_DIV_2);
   setup_psp(PSP_DISABLED);
   setup_spi(SPI_SS_DISABLED);
   setup_timer_0(RTCC_INTERNAL|RTCC_DIV_1);
   setup_timer_1(T1_DISABLED);
   setup_timer_2(T2_DISABLED,0,1);
   setup_comparator(NC_NC_NC_NC);
   setup_vref(FALSE);


{
output_high(verde1);
output_high(rojo2);
delay_ms(2000);
output_low(verde1);
output_high(ambar1);
delay_ms(500);
output_low(rojo2);
output_high(verde2);
delay_ms(1000);
output_low(ambar1);
output_high(rojo1);
delay_ms(2000);
output_low(verde2);
output_high(ambar2);
delay_ms(1000);
output_low(ambar2);
output_low(rojo1);

}
}
