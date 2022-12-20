# Ujian Akhir Semester 
Mata Kuliah 	:Dasar Pemrograman
Nama	      	:Supi Arianti
NIM		        :	1227050130
Jurusan		    :[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Matriks adalah sekumpulan bilangan yang disusun berdasarkan baris dan kolom, serta ditempatkan di dalam tanda kurung. Tanda kurungnya ini bisa berupa kurung biasa “( )” atau kurung siku “[ ]”. Suatu matriks diberi nama dengan huruf kapital, seperti A, B, C, dan seterusnya. Bedanya baris dan kolom adalah baris itu susunannya horizontal atau ke samping, sedangkan kolom susunannya vertikal atau dari atas ke bawah. 

## Source Code
NO 1
#include <iostream>
using namespace std;


int main()
{
int A[4][4];
int b,k,i,j,t,kolom,baris,angka;

cout <<"Jumlah baris : ";
cin >>baris;
cout <<"Jumlah kolom : ";
cin >>kolom;

{
    for(i=0; i< baris;i++)
    {
        for(j=0;j <kolom;j++)
        {
            cout <<"Nilai Matrik pada A [i] [j] : ";
            cin >> A[i][j] ;
        }
    }
    cout <<"\n Sebelum Berubah :\n";
        for(i=0;i<baris;i++)
    {
        for(j=0;j<kolom;j++)
        {
            cout<<A[i][j];
        }
        cout <<"\n";
    }

cout <<"\n Sesudah Berubah :\n";
        for(i=0;i<kolom;i++)
    {
        for(j=0;j<baris;j++)
        {
            cout<<A[j][i];
        }
        cout <<"\n";
    }
}

{
    cout <<"Baris jadi kolom, Kolom jadi baris";
}
return 0;
}

NO 2
#include <iostream>
using namespace std;
int main(){

     
     int matrika [3][2];
     int matrikb [3][2] = {{3,3},{5,5},{7,7}};
     int matrikc [3][2];

     
     int i,j;

     cout<<"\t===============================";
     cout<<"\n\t= Menampilkan bilangan yang habis dibagi 3,5,7, =\n";
     cout<<"\t===============================\n\n";

     
     
     for(i=0;i<3;i++){
          for(j=0;j<2;j++){
               cout<<"matrik a  ["<<i<<"] ["<<j<<"]  ";
               cin>>matrika[i][j];
          }
     }

     cout<<endl;

     
     for(i=0;i<3;i++){
          for(j=0;j<3;j++){
               matrikc[i][j]=matrika[i][j] / matrikb[i][j]; 
          }
     }

     
     cout<<"\nMatrik a\n";
     for(i=0;i<3;i++){
          for(j=0;j<2;j++){
               cout<<matrika[i][j]<<" ";
          }
          cout<<endl;
     }

     
     cout<<"\nMatrik b\n";
     for(i=0;i<3;i++){
          for(j=0;j<2;j++){
               cout<<matrikb[i][j]<<" ";
          }
          cout<<endl;
     }

     
     cout<<"\nMatrik c atau hasil\n";
     for(i=0;i<3;i++){
          for(j=0;j<2;j++){
               cout<<matrikc[i][j]<<" ";
          }
          cout<<endl;
     }

     return 0;
}
    
## Output
 NO 1
Jumlah baris : 2
Jumlah kolom : 3
Nilai Matrik pada A [i] [j] : 3
Nilai Matrik pada A [i] [j] : 4
Nilai Matrik pada A [i] [j] : 5
Nilai Matrik pada A [i] [j] : 6
Nilai Matrik pada A [i] [j] : 7
Nilai Matrik pada A [i] [j] : 8

 Sebelum Berubah :
345
678

 Sesudah Berubah :
36
47
58
Baris jadi kolom, Kolom jadi baris
    
 NO 2
    ===============================
        = Menampilkan bilangan yang habis dibagi 3,5,7, =
        ===============================

matrik a  [0] [0]  3
matrik a  [0] [1]  1
matrik a  [1] [0]  5
matrik a  [1] [1]  1
matrik a  [2] [0]  7
matrik a  [2] [1]  1


Matrik a
3 1
5 1
7 1

Matrik b
3 3
5 5
7 7

Matrik c atau hasil
1 0
1 0
1 0

--------------------------------
