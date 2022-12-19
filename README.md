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
    
    
    cout <<"bilangan yang tidak apat dibagi (3,5,7) : " << endl;

    for(x = 0; x <bris ; x++){
     	for(y = 0; y <klom ; y++){
      		if(a[x][y] % 3 != 0 && a[x][y] % 5 != 0 && a[x][y] % 7 != 0) {
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
Baris 1 kolom - 1 : 2
Baris 1 kolom - 2 : 3

Baris 2 kolom - 1 : 4
Baris 2 kolom - 2 : 5

Baris 3 kolom - 1 : 6
Baris 3 kolom - 2 : 7

 Hasil
  2   3
  4   5
  6   7
bilangan yang tidak apat dibagi (3,5,7) :
  2
  4
```
