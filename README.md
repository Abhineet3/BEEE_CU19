CODE
BEEE Lab Projects

int c=2;
  int a,t;
int bp=LOW,ls=HIGH;
int b;
void setup()
{
  pinMode(8,INPUT);
  for(int i=1;i<7;i++)
  {
  pinMode(i, OUTPUT);
  }
}

void loop()
{
  b=analogRead(A0);
  a=digitalRead(8);
  delay(100);
  if(a==HIGH)
  {
    c++;
    delay(100);
  }
 
 if(b<300)
  {
    
 
  if((c%2)==0)
  {
    for(int i=1;i<7;i++)
  {digitalWrite(i,HIGH);
    delay(500);
  digitalWrite(i,LOW);}
  
  }
  else
  {
  for(int i=1;i<7;i++)
  {digitalWrite(i,HIGH);
    delay(1000);
  digitalWrite(i,LOW);}
  
     
 }
    
 }
  else{
  for(int i=0;i<7;i++)
    digitalWrite(i,LOW);}
}
