# MZIDAN_IF-B
# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Program
<br> Nama		: MUHAMAD ZIDAN
<br>NIM		:	1227050079
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
PROGRAM BARIS DAN KOLOM BANYAK DATA BILANGAN HABIS DIBAGI 3,5,7
## Source Code
```
#include <iostream>
#include <iomanip>

using namespace std;

int main(){
	int a[100][100];
	int bris,klom,x,y;
	
	cout<<"=====================_Program Kolom dan Baris_====================="<<endl;
	cout<<"TUGAS UAS DASAR PROGRAM"<<endl;
	cout<<"Nama : Muhamad Zidan"<<endl;
	cout<<"Nim : 1227050079"<<endl;
	cout<<"==================================================================="<<endl;

	cout<<"Masukan nilai baris :";
	cin>>bris;
	cout<<"Masukan nilai kolom :";
	cin>>klom;
	
	for(x = 0; x<bris; x++){
     	for(y = 0; y <klom; y++){
            cout << "Baris " <<x+1<<" kolom - "<<y+1<< " : ";
            cin >> a[x][y];
        }
        cout << endl;
    }

    cout << " Hasil " << endl;

    for(x = 0; x <bris; x++){
    	for(y = 0; y <klom; y++){
        	cout <<setw(3)<<a[x][y] << " ";
    	}
    cout << endl;
    }
    
    
    cout <<"bilangan yang habis dibagi (3,5,7) : " << endl;

    for(x = 0; x <bris ; x++){
     	for(y = 0; y <klom ; y++){
      		if(a[x][y] % 3 == 0 || a[x][y] % 5 == 0 || a[x][y] % 7 == 0) {
        		cout <<setw(3)<<a[x][y] << " ";
        }
    }
    cout << endl;
    }
    return 0;
}
```
## Output
```
=====================_Program Kolom dan Baris_=====================
TUGAS UAS DASAR PROGRAM
Nama : Muhamad Zidan
Nim : 1227050079
===================================================================
Masukan nilai baris :3
Masukan nilai kolom :2
Baris 1 kolom - 1 : 10
Baris 1 kolom - 2 : 12

Baris 2 kolom - 1 : 20
Baris 2 kolom - 2 : 6

Baris 3 kolom - 1 : 8
Baris 3 kolom - 2 : 9

 Hasil
 10  12
 20   6
  8   9
bilangan yang habis dibagi (3,5,7) :
 10  12
 20   6
  9
```
