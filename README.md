# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		      : Dika Haekal Firza Pratama
<br>NIM		        :	1227050036
<br>Jurusan		    :[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Tema utama dari source code yang satu ini adalah untuk membuat array dalam implementasi deret aritmatika.
Tujuan utama dari source code ini adalah untuk mencari bilangan yang tidak habis dibagi angka 3,5 dan 7
Algoritma dari Source code ini yaitu :
1. User menginputkan berapa banyak baris pada array mulai dari range 0-20.
2. User menginputkan berapa banyak baris pada array mulai dari range 0-20.
3. User menginputkan satu persatu nilai array,dimulai dari baris 1 dan kolom 1.
4. Jika sudah,Nilai dalam array tersebut di tampilkan sesuai aturan matriks.
5. Kemudian nilai divalidasi kembali apakah nilai tersebut habis dibagi 3,5 dan 7.
6. Apabila nilai tadi habis dibagi 3,5 dan 7, maka nilai tidak akan ditampilkan. apabila tidak habis. tampilkan kembali kepada user

## Source Code

	#include <iostream>
	using namespace std;
	void garis(){
	cout << "=======================================" << endl;}
	int main (){
	garis();
	int A [20][20];
	int b, k, i, j;
	cout << "Imputkan berapa banyak baris yang ingin di imputkan : ";
	cin >> b;
	cout << "Imputkan berapa banyak kolom yang ingin di imputkan : ";
	cin >> k;
	garis();
	for (i=0;i<=b-1;i++) {
		for(j=0;j<=k-1;j++) {
			cout << "Masukkan nilai (" << i << "." << j << ") : ";
			cin >> A [i][j];
		}
		garis();
	}
	cout << "Nilai yang diinputkan : \n";
	for(int i = 0; i < b; i++){
		for(int j = 0; j < k; j++){
			cout<<A[i][j]<<"\t";
		}
		cout<<endl;
	}
	int angka[20];
	int index = 0;
	for(i=0;i<b;i++){
		for(j=0;j<k;j++) {
			if (A [i][j]%3 != 0 && A[i][j]%5 != 0 && A[i][j]%7 != 0){
				angka[index] = A[i][j];
				index++;
			}
		}
	}
	cout<<"Angka yang tidak bisa dibagi 3, 5, 7 adalah ";
	for(int i = 0; i < index; i++){
		cout<<angka[i]<<" ";
	}
	}

## Output
![uas deret array](https://user-images.githubusercontent.com/121142632/209270125-8745f550-7def-43ac-92ce-5faf0d8f80f0.png)
