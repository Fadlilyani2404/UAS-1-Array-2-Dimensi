# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Fadlil Yani Aini Syamsi
<br>NIM		:	1227050041
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Tema utama dari source code yang satu ini adalah untuk membuat array 2 dimensi menggunakan bahasa C++.<br>
Tujuan utama dari source code ini adalah mengubah letak nilai yang tadinya sebuah baris menjadi sebuah kolom, begitupun sebaliknya.</br>
Algoritma dari Source code ini yaitu : <br>
<ol>
<li>User menginputkan berapa banyak baris pada array.</li>
<li>User menginputkan berapa banyak kolom dari baris pada array.</li>
<li>User menginputkan satu persatu nilai array,dimulai dari baris 1 dan kolom 1.</li>
<li>Jika sudah,Nilai dalam array tersebut di tampilkan sesuai aturan matriks.</li>
<li>Lalu ditampilkan juga nilai dalam array yang sudah dibalik,dari baris menjadi kolom dan sebaliknya.</li>
</ol>

## Source Code
<code>
#include <iostream>
#include <conio.h>
using namespace std;

void garis(){
	cout<<"--------------------------------------"<<endl;
}

main(){
	int br,kl,x,y,z;
	cout<<"Inputkan berapa banyak baris yang diinginkan untuk array : ";
	cin>>br;
	cout<<"Inputkan berapa banyak kolom yang diinginkan untuk array : ";
	cin>>kl;
	garis();
	
	int array[br][kl],tukar[br][kl]; 
    cout<<"Berikan nilai pada array!"<<endl;
    garis();
    for (x=1; x<=br; x++){
    	for(y=1; y<=kl; y++){
    		cout<<"Array baris ke-"<<x<<" kolom ke-"<<y<<": \n";
    		cin>>array[x][y];
    		garis();
		}
	}
	
	cout<<"Array sebelum ditukar kolom dan barisnya : \n";
	garis();
	for(x=1;x<=br;x++){
		for(y=1;y<=kl;y++){
			cout<<"  "<<array[x][y];
		}
		cout<<endl;
	}
	garis();
	
	cout<<"Array sesudah ditukar kolom dan barisnya : \n";
	garis();
	for(x=1;x<=kl;x++){
		for(y=1;y<=br;y++){
			cout<<"  "<<array[y][x];
		}
		cout<<endl;
	}
	garis();
}
</code>

## Output
![Output UAS 1](https://user-images.githubusercontent.com/113232952/209470761-b0b9ac07-c4ad-4553-8436-1f777da0f3fd.png)
