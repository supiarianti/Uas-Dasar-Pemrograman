# Ujian Akhir Semester 
Mata Kuliah 	:Dasar Pemrograman
Nama	      	:Supi Arianti
NIM		        :	1227050130
Jurusan		    :[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Matriks adalah sekumpulan bilangan yang disusun berdasarkan baris dan kolom, serta ditempatkan di dalam tanda kurung. Tanda kurungnya ini bisa berupa kurung biasa “( )” atau kurung siku “[ ]”. Suatu matriks diberi nama dengan huruf kapital, seperti A, B, C, dan seterusnya. Bedanya baris dan kolom adalah baris itu susunannya horizontal atau ke samping, sedangkan kolom susunannya vertikal atau dari atas ke bawah. 

## Source Code
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

## Output
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
