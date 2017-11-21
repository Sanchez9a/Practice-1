#ifndef DADOS_H
	#define DADOS_H
	#include <vector>
	#include <cstdlib>
	#include <ctime>
  using namespace std;
  
  class Dados{
  
  private:
      int d1_;
      int d2_;
      
      int lanzamiento1_;
      int lanzamiento2_;
      
      int suma1_;
      int suma2_;
      
      <vector> int v1_, v2_;
  
      void push1();
      void push2();
      
      
   public:
   
   Dados();
   void lanzamiento();
   inline int getdado1() {return d1_;};
   inline int getdado2() {return d2_;};
   bool setdado1(int dado);
   bool setdado2(int dado);
   inline int getsuma() {return d1_+d2_;};
   inline int getdiferencia() {if(d2_>d1_) {return d2_-d1_;}; else {return d1_-d2_;};
   inline int getLanzamientos1() {return lanzamientos1_;};
	 inline int getLanzamientos2() {return lanzamientos2_;};
	 float getMedia1();
	 float getMedia2();

	 inline void getUltimos1(int v[]) {for(int i=0;i<5;i++) v[i]=v1_[i];};
	 inline void getUltimos2(int v[]) {for(int i=0;i<5;i++) v[i]=v2_[i];};

	};

#endif
       
  
