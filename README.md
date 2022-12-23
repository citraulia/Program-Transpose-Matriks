# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama : CITRA AULIA
<br>NIM : 1227050030
<br>Jurusan		: [Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
<br> Kali ini Kita akan membuat program transpose matriks yaitu mengubah posisi baris menjadi kolom dan kolom menjadi baris dengan menggunakan bahasa c++. Untuk program ini Kita dapat menggunakan array 2 dimensi dan pengulangan for.

<br> Pada langkah awal, program meminta 2 inputan awal untuk berupa jumlah baris dan jumlah kolom pada array, kemudian setelah itu, program akan meminta untuk memasukkan satu per satu angka untuk baris dan kolom pada array sesuai dengan jumlah baris dan kolom tadi.

<br> Selanjutnya program akan menampilkan hasil inputan tadi dan hasil setelah nilai inputan dibalik yaitu baris menjadi kolom dan begitu pula sebaliknya.

## Source Code
```cpp
#include <iostream>
#include <iomanip>
using namespace std;
 
int main()
{
	int matriks[100][100];
	int baris, kolom, i, j;
  
	cout << "Program Transpose Matriks\n" << endl;
	
	cout << "Masukan jumlah baris: "; cin >> baris;
	cout << "Masukan jumlah kolom: "; cin >> kolom;
	cout << endl;
 
	for(i = 0; i < baris ; i++){
    	for(j = 0; j < kolom; j++){
      		cout << "Baris " <<i+1<<", kolom "<<j+1<< " = ";
      		cin >> matriks[i][j];
		}
	}
	
	cout << endl;
 	cout << "Nilai Input: " << endl;
 
	for(i = 0; i < baris ; i++){
		for(j = 0; j < kolom; j++){
			cout << matriks[i][j] << " ";
  	  }
    cout << endl;
	}
 
	cout << endl;
	cout << "Hasil Setelah Diubah: " << endl;
	for(i = 0; i < kolom ; i++){
		for(j = 0; j < baris; j++){
    		cout << matriks[j][i] << " ";
   		}
	cout << endl;
	}
  
	 return 0;
}
```

## Output
![img 1](https://user-images.githubusercontent.com/121267209/209328139-117aa7f7-91d9-40d9-9d6c-42e1a47a0721.png)
