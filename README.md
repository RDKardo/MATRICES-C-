# MATRICES-C-
Multiplicacion de Matrices 3x3 en c++
#include <iostream>
#define d 3
using std::cout;
using std::cin;
using std::endl;

int main(){
    int i, j, k, a[d][d], b[d][d], c[d][d];
    cout << "MATRIZ A." << endl;
    for(i = 0 ; i < d ; i++){
        for(j = 0 ; j < d ; j++){
     cout << "Introduzca el valor del elemento [" << i << "]["
      << j << "]: ";
     cin >> a[i][j];
 }
    }
    cout << endl;
    for(i = 0 ; i < d ; i++){
        for(j = 0 ; j < d ; j++){
            cout << a[i][j] << " ";
            if(j == 2)
               cout << endl;
    }
    }
    cout << endl;
    cout << "MATRIZ B." << endl;
    for(i = 0 ; i < d ; i++){
        for(j = 0 ; j < d ; j++){
            cout << "Introduzca el valor del elemento[" << i << "]["
                    << j << "]: ";
            cin >> b[i][j];
        }
    }
    cout << endl;
    for(i = 0 ; i < d ; i++){
        for(j = 0 ; j < d ; j++){
            cout << b[i][j] << " ";
            if(j == 2)
               cout << endl;
        }
    }
  for(i=0;i<d;i++){
      for(j=0;j<d;j++){
          c[i][j]=0;
          for(k=0;k<d;k++){
              c[i][j]=c[i][j]+(a[i][k]*b[k][j]);
          }
      }
  }
  cout << endl << "MATRIZ C (Matriz A*B)." << endl;
  cout << endl;
  for(i=0;i<d;i++){
      for(j=0;j<d;j++){
          cout << c[i][j] << " ";
          if(j==2)
             cout << endl;
      }
  }


  return 0;
  }
