int pwm=11 ;
void setup() {
  // put your setup code here, to run once:
  pinMode(pwm,OUTPUT);

}

void loop() {
  // put your main code here, to run repeatedly:
for(int i=0;i<=255;i++)
{
analogWrite(pwm,i);
delay(10);
}
for(int i=255;i>=0;i--)
{
analogWrite(pwm,i);
delay(10);
}
}
