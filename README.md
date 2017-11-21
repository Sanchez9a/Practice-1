#include "dados.h"

Dados::Dados(){
   srand(time(NULL));
   d1_=1;
   d2_=1;
   lanzamientos1_=0;
   lanzamientos2_=0;
   suma1_=0;
   suma2_=0;
   v1_.resize(5,0);
   v2_.resize(5,0);
}



