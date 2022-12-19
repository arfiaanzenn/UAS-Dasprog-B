# Ujian Akhir Semester 
<br>Mata Kuliah 	: Dasar Pemrograman
<br> Nama		: Muhammad Farhan Tarigan
<br>NIM		:	1227050089
<br>Jurusan		:[Teknik Informatika](http://if.uinsgd.ac.id/) [UIN Sunan Gunung Djati Bandung](https://uinsgd.ac.id/) 

## Deskripsi Umum
Matriks merupakan kumpulan-kumpulan bilangan yang disusun secara baris (vertikal) dan kolom (horizontal), bisa juga disebut dengan array dua dimensi (multi-dimensional). Adapun Transpose Matriks adalah memperoleh sebuah matriks dengan cara menukar baris menjadi kolom dan kolom menjadi baris dari sebuah matriks.

## Source Code 1
    #include <iostream>
    using namespace std;

    int main() {
     int arr[100][100], transpose[100][100], baris, kolom;

      cout << "Nama : Muhammad Farhan Tarigan" << endl;
      cout << "NIM : 1227050089" << endl;
      cout << "Kelas : IF 22 - B" << endl;
      cout << "=======================================" << endl;
      cout << "^Program C++ Transpose Matrix Ordo 2^" << endl;
      cout << "=======================================" << endl;

     cout << "baris: "; cin >> baris;
     cout << "kolom: "; cin >> kolom;

     for(int i=0; i<baris; i++){
      for(int j=0; j<kolom; j++){
       cout << "arr ke["<<i <<"."<<j<<"]: "; cin >> arr[i][j];
      }
     }

     cout << endl;

     for(int i=0; i<baris; i++){
      for(int j=0; j<kolom; j++){
       cout << arr[i][j] << " ";
       if(j == kolom - 1);
      }
      cout << endl;
     }

     cout << endl;

     for(int i=0; i<baris; i++){
      for(int j=0; j<kolom; j++){
       transpose[j][i] = arr[i][j];
      }
     }

     for(int i=0; i<kolom; i++){
      for(int j=0; j<baris; j++){
       cout << transpose[i][j] << " ";
       if(j == baris - 1);
      }
      cout << endl;
     }
    }
    
## Source Code 2
    #include <iostream>

    using namespace std;

    int main() {
       int matrix[100][100], baris, kolom, num;

       cout << "Nama : Muhammad Farhan Tarigan" << endl;
      cout << "NIM : 1227050089" << endl;
      cout << "Kelas : IF 22 - B" << endl;
      cout << "=======================================" << endl;
      cout << "^Program C++ Matrix Ordo 2 habis dibagi 3 5 7^" << endl;
      cout << "=======================================" << endl;
      // Membuat matriks dengan ukuran 


       cout << "baris: "; cin >> baris;
     cout << "kolom: "; cin >> kolom;

      // Menambahkan elemen ke dalam matriks
      for (int i = 0; i < baris; i++) {
        for (int j = 0; j < kolom; j++) {

        cout << "Matriks ke["<<i <<"."<<j<<"]: ";
          cin >> num;
          // Menambahkan elemen ke dalam matriks jika habis dibagi oleh 3, 5, atau 7
          if (num % 3 == 0 || num % 5 == 0 || num % 7 == 0) {
            matrix[i][j] = num;
          }
        }
      }

      // Mencetak matriks
      for (int i = 0; i < baris; i++) {
        for (int j = 0; j < kolom; j++) {
          cout << matrix[i][j] << " ";
        }
        cout << endl;
      }

      return 0;
    }

## Output 1

![Screenshot (22)](https://user-images.githubusercontent.com/120624265/208393763-5d434513-b32b-4398-990b-762e7922e151.png)



## Output 2

![Screenshot (23)](https://user-images.githubusercontent.com/120624265/208393798-ce50278a-6457-438e-a083-3b550134661f.png)

